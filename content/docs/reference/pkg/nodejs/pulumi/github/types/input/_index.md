---
title: "Module types/input"
title_tag: "Module types/input | Package @pulumi/github | Node.js SDK"
linktitle: "input"
meta_desc: "Explore members of the input module in the @pulumi/github package."
git_sha: "3d749903fe0c79eacbbeca6c6550682fc3d7eb4c"
---

<!-- WARNING: this page was generated by a tool. Do not edit it by hand. -->
<!-- To change it, please see https://github.com/pulumi/docs/tree/master/tools/tscdocgen. -->






<h3>APIs</h3>
<ul class="api">
    <li><a href="#BranchProtectionRequiredPullRequestReviews"><span class="symbol api"></span>BranchProtectionRequiredPullRequestReviews</a></li>
    <li><a href="#BranchProtectionRequiredStatusChecks"><span class="symbol api"></span>BranchProtectionRequiredStatusChecks</a></li>
    <li><a href="#BranchProtectionRestrictions"><span class="symbol api"></span>BranchProtectionRestrictions</a></li>
    <li><a href="#OrganizationWebhookConfiguration"><span class="symbol api"></span>OrganizationWebhookConfiguration</a></li>
    <li><a href="#RepositoryTemplate"><span class="symbol api"></span>RepositoryTemplate</a></li>
    <li><a href="#RepositoryWebhookConfiguration"><span class="symbol api"></span>RepositoryWebhookConfiguration</a></li>
</ul>




<h2 id="apis">APIs</h2>
<h3 class="pdoc-module-header" id="BranchProtectionRequiredPullRequestReviews" data-link-title="BranchProtectionRequiredPullRequestReviews">
    <a href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L7">
        interface <strong>BranchProtectionRequiredPullRequestReviews</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>BranchProtectionRequiredPullRequestReviews</span></code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredPullRequestReviews-dismissStaleReviews">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L8">property <b>dismissStaleReviews</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>dismissStaleReviews?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredPullRequestReviews-dismissalTeams">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L9">property <b>dismissalTeams</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>dismissalTeams?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredPullRequestReviews-dismissalUsers">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L10">property <b>dismissalUsers</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>dismissalUsers?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredPullRequestReviews-includeAdmins">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L11">property <b>includeAdmins</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>includeAdmins?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredPullRequestReviews-requireCodeOwnerReviews">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L12">property <b>requireCodeOwnerReviews</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>requireCodeOwnerReviews?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredPullRequestReviews-requiredApprovingReviewCount">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L13">property <b>requiredApprovingReviewCount</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>requiredApprovingReviewCount?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number'>number</a></span>&gt;;</code></pre>
<h3 class="pdoc-module-header" id="BranchProtectionRequiredStatusChecks" data-link-title="BranchProtectionRequiredStatusChecks">
    <a href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L16">
        interface <strong>BranchProtectionRequiredStatusChecks</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>BranchProtectionRequiredStatusChecks</span></code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredStatusChecks-contexts">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L17">property <b>contexts</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>contexts?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredStatusChecks-includeAdmins">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L18">property <b>includeAdmins</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>includeAdmins?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRequiredStatusChecks-strict">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L19">property <b>strict</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>strict?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>
<h3 class="pdoc-module-header" id="BranchProtectionRestrictions" data-link-title="BranchProtectionRestrictions">
    <a href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L22">
        interface <strong>BranchProtectionRestrictions</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>BranchProtectionRestrictions</span></code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRestrictions-apps">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L23">property <b>apps</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>apps?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRestrictions-teams">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L24">property <b>teams</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>teams?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</code></pre>
<h4 class="pdoc-member-header" id="BranchProtectionRestrictions-users">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L25">property <b>users</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>users?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;[]&gt;;</code></pre>
<h3 class="pdoc-module-header" id="OrganizationWebhookConfiguration" data-link-title="OrganizationWebhookConfiguration">
    <a href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L28">
        interface <strong>OrganizationWebhookConfiguration</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>OrganizationWebhookConfiguration</span></code></pre>
<h4 class="pdoc-member-header" id="OrganizationWebhookConfiguration-contentType">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L29">property <b>contentType</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>contentType?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="OrganizationWebhookConfiguration-insecureSsl">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L30">property <b>insecureSsl</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>insecureSsl?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="OrganizationWebhookConfiguration-secret">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L31">property <b>secret</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>secret?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="OrganizationWebhookConfiguration-url">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L35">property <b>url</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>url: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

URL of the webhook

<h3 class="pdoc-module-header" id="RepositoryTemplate" data-link-title="RepositoryTemplate">
    <a href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L38">
        interface <strong>RepositoryTemplate</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>RepositoryTemplate</span></code></pre>
<h4 class="pdoc-member-header" id="RepositoryTemplate-owner">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L39">property <b>owner</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>owner: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="RepositoryTemplate-repository">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L40">property <b>repository</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>repository: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>
<h3 class="pdoc-module-header" id="RepositoryWebhookConfiguration" data-link-title="RepositoryWebhookConfiguration">
    <a href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L43">
        interface <strong>RepositoryWebhookConfiguration</strong>
    </a>
</h3>

<pre class="highlight"><code><span class='kr'>interface</span> <span class='nx'>RepositoryWebhookConfiguration</span></code></pre>
<h4 class="pdoc-member-header" id="RepositoryWebhookConfiguration-contentType">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L44">property <b>contentType</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>contentType?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="RepositoryWebhookConfiguration-insecureSsl">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L45">property <b>insecureSsl</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>insecureSsl?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Boolean'>boolean</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="RepositoryWebhookConfiguration-secret">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L46">property <b>secret</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>secret?: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>
<h4 class="pdoc-member-header" id="RepositoryWebhookConfiguration-url">
<a class="pdoc-child-name" href="https://github.com/pulumi/pulumi-github/blob/3d749903fe0c79eacbbeca6c6550682fc3d7eb4c/sdk/nodejs/types/input.ts#L50">property <b>url</b></a>
</h4>

<pre class="highlight"><code><span class='kd'></span>url: <a href='/docs/reference/pkg/nodejs/pulumi/pulumi/#Input'>pulumi.Input</a>&lt;<span class='kd'><a href='https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String'>string</a></span>&gt;;</code></pre>

URL of the webhook
