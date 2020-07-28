# Learn Pulumi

So you're interested in writing some Learn Pulumi content? Great! Follow these
steps to make it happen.

## Setting up your development environment

If you haven't done so already, clone this repository and
[follow the instructions in the README](https://github.com/pulumi/docs#pulumi-documentation-site)
to set up your `pulumi/docs` development environment and run the development web server.

Once you're able to run:

```zsh
$ make serve
```

... you can browse the site locally at http://localhost:1313/, and any changes you make to the pages of the site will be reloaded automatically in your browser.

## How Learn content is organized

All content lives under `./content/learn`. Modules, which appear as cards on the Learn home page, sit at the top level of the `learn` folder, and each of the topics that comprise a given module live as siblings underneath their parent module. There are only these two levels in the hierarchy; no further nesting is supported as of today.

```
$ tree ./content/learn

./content/learn
├── _index.md
└── pulumi-101-aws
    ├── projects-and-stacks
    │   ├── index.md
    │   └── meta.png
    ├── configuration-and-secrets
    │   ├── index.md
    │   └── meta.png
    │   ...
    ├── meta.png
    └── _index.md
```

You can control the order in which modules appear on the Learn home page by adjusting the value of the `index` property in the module's YAML frontmatter:

```
---
title: "Pulumi 101 on AWS"
layout: module
...

# The order in which the module appears on the home page.
index: 0
...
```

Similarly, you can control the sort order of topics within a given module by adjusting their `index` properties as well:

```
---
title: "Projects and Stacks"
layout: topic
...

# The order in which the topic appears in the module.
index: 0
...
```

## Creating new modules or topics

We have a couple of helpers that make it easy to create new modules and topics. Please use them! **Please don't copy and paste content from other modules or topics to create new ones.** If (er, when) you have trouble with one of the helpers, [file an issue](issues) so we can address it and make the authoring process better.

### Creating a new module

When you know what you want to call the new module, make sure you're at the root of the `docs` repository, then run the new-module helper as below. (You can do this anytime; you don't have to be running the development server.)

```
$ make new_learn_module
```

The helper will prompt you for a _slug_ -- a URL-friendly name that'll be used as the path to the module under `/learn`. Enter a name, such as `pulumi-101-aws` or `pulumi-101-azure`, and hit Enter. (You can always rename the folder of the module later, so don't worry if you don't pick the perfect thing on the first try.)

```
$ make new_learn_module
...

Module name (e.g., pulumi-101-aws): pulumi-101-azure
docs/content/learn/pulumi-101-azure created
```

Hugo will do its best to convert the slug to a proper title -- e.g., `pulumi-101-azure` becomes `Pulumi 101 Azure` -- but if you find that the conversion looks a bit weird, or you just want to change it to something else, you can do that by editing the module file's YAML frontmatter directly.

Since a module should have at least one topic, the generator will then prompt you for a new topic as well. Give it a URL-friendly name, in the same way you did with the module, and it'll be created as a folder with that name under the module.

```
$ make new_learn_module
...

Module name (e.g., pulumi-101-aws): pulumi-101-azure
docs/content/learn/pulumi-101-azure created

...
Topic name (e.g., basics): basics
docs/content/learn/pulumi-101-azure/basics created
```

When you want to create a topic for a module that already exists, use the topic-specific helper:

```
$ make new_learn_topic
```

The new-topic helper needs to know what module your new topic should belong to, so you'll need to give it the name of the folder that contains it -- for example, to create a new topic for the `pulumi-101-azure` module, enter `pulumi-101-azure`:

```
$ make new_learn_topic
...

Module name (e.g., pulumi-101-aws): pulumi-101-azure
Topic name (e.g., basics): advanced-basics
docs/content/learn/pulumi-101-azure/advanced-basics created
```

At this point, your new topic is created and you're ready to start writing. Each file should contain annotated frontmatter explaining how each property works, and if you find you don't have something you need, feel free to reach out in the #docs channel.

## What's a module? What's a topic?

A topic is a single focused lesson aimed at teaching someone how to do something -- ideally, something that can be completed in a relatively short period of time, like 30 minutes or less.

A module is a collection of topics that share a common theme and that are organized (usually linearly) in the interest of teaching a subject that's not easily covered in a single tutorial, example, or blog post.

### How do they differ from tutorials and examples?

These definitions aren't perfect, but they should hopefully help to clarify answer that question.

* An **example** is single Pulumi program (or perhaps the same program in multiple languages) with a concise README and a maybe [Deploy with Pulumi button](https://www.pulumi.com/docs/intro/console/extensions/pulumi-button/). Examples are meant to serve as reference content; they're like snapshots of a finished product. Most of the programs in the [examples repo](https://github.com/pulumi/examples) today fall into this category.

* A **tutorial** is a guided walkthrough that might end with a finished example. Like a blog post, it's written in a familiar tone, generally in the second person ("you/your"), and it's aimed at having the reader learn something by doing. Whereas an example might say, _Here's the finished thing_, a tutorial says, _Let's build this thing together_.

* A **module** more like a chapter in a book, its topics like sections within that chapter. Stylistically, a topic may be written like a tutorial, but a topic may not end with a concrete result; instead, a topic might just tell you how to do something or how something works.

| Content Type    | Representative Title |
| --------------- | -------------------------------------------------------- |
| Example         | Simple static website with Pulumi and Amazon S3          |
| Tutorial        | Building a video-processing service with Pulumi and AWS  |
| Module & topics | Strategies for testing your infrastructure code          |

Again, these aren't perfect, and not set in stone. They're just meant to serve as a guide.

## Conventions, briefly

* Try to keep to vanilla Markdown and Hugo shortcodes. If you find you need more than you can express with these, let us know, and we'll do our best to get you what you need.

* Don't try to do too much with a single module or topic. Small modules, and short, focused topics are great. People are busy -- respect their time. Content-wise, in general, opt for provider-specific modules as opposed to higher-level ones; for example, `pulumi-101-aws` and `pulumi-101-azure`, rather than just a single `pulumi-101` that tries to cover both providers.

* Keep it simple and maintainable. Multiple languages represented within a single topic is fine, of course. Multiple languages, within multiple clouds, within a single topic is going to be painful for you to write and even more painful for others to maintain.

## Questions?

Ping Christian or anyone in the #docs channel.
