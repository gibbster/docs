---
title: Package pulumi_fastly
title_tag: Package pulumi_fastly | Python SDK
linktitle: pulumi_fastly
notitle: true
block_external_search_index: true
---

{{< resource-docs-alert "fastly" >}}

<div class="section" id="pulumi-fastly">
<h1>Pulumi Fastly<a class="headerlink" href="#pulumi-fastly" title="Permalink to this headline">¶</a></h1>
<blockquote>
<div><p>This provider is a derived work of the <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-fastly">Terraform Provider</a> distributed under
<a class="reference external" href="https://www.mozilla.org/en-US/MPL/2.0/">MPL 2.0</a>. If you encounter a bug or missing feature, first check the
<a class="reference external" href="https://github.com/pulumi/pulumi-fastly/issues">pulumi/pulumi-fastly repo</a>; however, if that doesn’t turn up
anything, please consult the source <a class="reference external" href="https://github.com/terraform-providers/terraform-provider-fastly/issues">terraform-providers/terraform-provider-fastly repo</a>.</p>
</div></blockquote>
<span class="target" id="module-pulumi_fastly"></span><dl class="py class">
<dt id="pulumi_fastly.AwaitableGetFastlyIpRangesResult">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">AwaitableGetFastlyIpRangesResult</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">cidr_blocks</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">id</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">ipv6_cidr_blocks</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.AwaitableGetFastlyIpRangesResult" title="Permalink to this definition">¶</a></dt>
<dd></dd></dl>

<dl class="py class">
<dt id="pulumi_fastly.GetFastlyIpRangesResult">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">GetFastlyIpRangesResult</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">cidr_blocks</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">id</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">ipv6_cidr_blocks</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.GetFastlyIpRangesResult" title="Permalink to this definition">¶</a></dt>
<dd><p>A collection of values returned by getFastlyIpRanges.</p>
<dl class="py method">
<dt id="pulumi_fastly.GetFastlyIpRangesResult.cidr_blocks">
<em class="property">property </em><code class="sig-name descname">cidr_blocks</code><a class="headerlink" href="#pulumi_fastly.GetFastlyIpRangesResult.cidr_blocks" title="Permalink to this definition">¶</a></dt>
<dd><p>The lexically ordered list of ipv4 CIDR blocks.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.GetFastlyIpRangesResult.id">
<em class="property">property </em><code class="sig-name descname">id</code><a class="headerlink" href="#pulumi_fastly.GetFastlyIpRangesResult.id" title="Permalink to this definition">¶</a></dt>
<dd><p>The provider-assigned unique ID for this managed resource.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.GetFastlyIpRangesResult.ipv6_cidr_blocks">
<em class="property">property </em><code class="sig-name descname">ipv6_cidr_blocks</code><a class="headerlink" href="#pulumi_fastly.GetFastlyIpRangesResult.ipv6_cidr_blocks" title="Permalink to this definition">¶</a></dt>
<dd><p>The lexically ordered list of ipv6 CIDR blocks.</p>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_fastly.Provider">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">Provider</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">api_key</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">base_url</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Provider" title="Permalink to this definition">¶</a></dt>
<dd><p>The provider type for the fastly package. By default, resources use package-wide configuration
settings, however an explicit <code class="docutils literal notranslate"><span class="pre">Provider</span></code> instance may be created and passed during resource
construction to achieve fine-grained programmatic control over provider settings. See the
<a class="reference external" href="https://www.pulumi.com/docs/reference/programming-model/#providers">documentation</a> for more information.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>api_key</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Fastly API Key from <a class="reference external" href="https://app.fastly.com/#account">https://app.fastly.com/#account</a></p></li>
<li><p><strong>base_url</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Fastly API URL</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_fastly.Provider.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Provider.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Provider.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Provider.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_fastly.ServiceACLEntriesv1">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">ServiceACLEntriesv1</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">acl_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">entries</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceACLEntriesv1EntryArgs, Mapping[str, Any], Awaitable[Union[ServiceACLEntriesv1EntryArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceACLEntriesv1EntryArgs, Mapping[str, Any], Awaitable[Union[ServiceACLEntriesv1EntryArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">service_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceACLEntriesv1" title="Permalink to this definition">¶</a></dt>
<dd><p>Defines a set of Fastly ACL entries that can be used to populate a service ACL.  This resource will populate an ACL with the entries and will track their state.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">config</span> <span class="o">=</span> <span class="n">pulumi</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
<span class="n">myacl_name</span> <span class="o">=</span> <span class="n">config</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;myaclName&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">myacl_name</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
    <span class="n">myacl_name</span> <span class="o">=</span> <span class="s2">&quot;My ACL&quot;</span>
<span class="n">myservice</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1</span><span class="p">(</span><span class="s2">&quot;myservice&quot;</span><span class="p">,</span>
    <span class="n">domains</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DomainArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com&quot;</span><span class="p">,</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">backends</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
        <span class="n">address</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com.s3-website-us-west-2.amazonaws.com&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;AWS S3 hosting&quot;</span><span class="p">,</span>
        <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">acls</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1AclArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="n">myacl_name</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">force_destroy</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">entries</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">ServiceACLEntriesv1</span><span class="p">(</span><span class="s2">&quot;entries&quot;</span><span class="p">,</span>
    <span class="n">service_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">id</span><span class="p">,</span>
    <span class="n">acl_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">acls</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="n">acls</span><span class="p">:</span> <span class="p">{</span><span class="n">d</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">d</span><span class="o">.</span><span class="n">acl_id</span> <span class="k">for</span> <span class="n">d</span> <span class="ow">in</span> <span class="n">acls</span><span class="p">}[</span><span class="n">myacl_name</span><span class="p">]),</span>
    <span class="n">entries</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">ServiceACLEntriesv1EntryArgs</span><span class="p">(</span>
        <span class="n">ip</span><span class="o">=</span><span class="s2">&quot;127.0.0.1&quot;</span><span class="p">,</span>
        <span class="n">subnet</span><span class="o">=</span><span class="s2">&quot;24&quot;</span><span class="p">,</span>
        <span class="n">negated</span><span class="o">=</span><span class="kc">False</span><span class="p">,</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;ALC Entry 1&quot;</span><span class="p">,</span>
    <span class="p">)])</span>
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>acl_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the ACL that the items belong to</p></li>
<li><p><strong>entries</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceACLEntriesv1EntryArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Set ACL entries that are applied to the service. Defined below</p></li>
<li><p><strong>service_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the Service that the ACL belongs to</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_fastly.ServiceACLEntriesv1.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">acl_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">entries</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceACLEntriesv1EntryArgs, Mapping[str, Any], Awaitable[Union[ServiceACLEntriesv1EntryArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceACLEntriesv1EntryArgs, Mapping[str, Any], Awaitable[Union[ServiceACLEntriesv1EntryArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">service_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_fastly.service_acl_entriesv1.ServiceACLEntriesv1<a class="headerlink" href="#pulumi_fastly.ServiceACLEntriesv1.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ServiceACLEntriesv1 resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>acl_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the ACL that the items belong to</p></li>
<li><p><strong>entries</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceACLEntriesv1EntryArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Set ACL entries that are applied to the service. Defined below</p></li>
<li><p><strong>service_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the Service that the ACL belongs to</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceACLEntriesv1.acl_id">
<em class="property">property </em><code class="sig-name descname">acl_id</code><a class="headerlink" href="#pulumi_fastly.ServiceACLEntriesv1.acl_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the ACL that the items belong to</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceACLEntriesv1.entries">
<em class="property">property </em><code class="sig-name descname">entries</code><a class="headerlink" href="#pulumi_fastly.ServiceACLEntriesv1.entries" title="Permalink to this definition">¶</a></dt>
<dd><p>A Set ACL entries that are applied to the service. Defined below</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceACLEntriesv1.service_id">
<em class="property">property </em><code class="sig-name descname">service_id</code><a class="headerlink" href="#pulumi_fastly.ServiceACLEntriesv1.service_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the Service that the ACL belongs to</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceACLEntriesv1.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceACLEntriesv1.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceACLEntriesv1.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceACLEntriesv1.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_fastly.ServiceCompute">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">ServiceCompute</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">activate</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">backends</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeBackendArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBackendArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeBackendArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBackendArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">bigqueryloggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeBigqueryloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBigqueryloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeBigqueryloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBigqueryloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">blobstorageloggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeBlobstorageloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBlobstorageloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeBlobstorageloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBlobstorageloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">comment</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">domains</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeDomainArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeDomainArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeDomainArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeDomainArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">force_destroy</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">gcsloggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeGcsloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeGcsloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeGcsloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeGcsloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">healthchecks</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeHealthcheckArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeHealthcheckArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeHealthcheckArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeHealthcheckArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">httpsloggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeHttpsloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeHttpsloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeHttpsloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeHttpsloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logentries</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLogentryArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLogentryArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLogentryArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLogentryArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_cloudfiles</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingCloudfileArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingCloudfileArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingCloudfileArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingCloudfileArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_datadogs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingDatadogArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingDatadogArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingDatadogArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingDatadogArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_digitaloceans</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingDigitaloceanArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingDigitaloceanArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingDigitaloceanArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingDigitaloceanArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_elasticsearches</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingElasticsearchArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingElasticsearchArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingElasticsearchArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingElasticsearchArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_ftps</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingFtpArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingFtpArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingFtpArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingFtpArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_googlepubsubs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingGooglepubsubArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingGooglepubsubArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingGooglepubsubArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingGooglepubsubArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_heroku</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingHerokuArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingHerokuArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingHerokuArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingHerokuArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_honeycombs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingHoneycombArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingHoneycombArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingHoneycombArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingHoneycombArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_kafkas</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingKafkaArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingKafkaArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingKafkaArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingKafkaArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_logglies</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingLogglyArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingLogglyArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingLogglyArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingLogglyArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_logshuttles</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingLogshuttleArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingLogshuttleArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingLogshuttleArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingLogshuttleArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_newrelics</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingNewrelicArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingNewrelicArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingNewrelicArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingNewrelicArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_openstacks</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingOpenstackArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingOpenstackArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingOpenstackArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingOpenstackArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_scalyrs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingScalyrArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingScalyrArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingScalyrArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingScalyrArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_sftps</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingSftpArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingSftpArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingSftpArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingSftpArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">name</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">package</span><span class="p">:</span> <span class="n">Union[ServiceComputePackageArgs, Mapping[str, Any], Awaitable[Union[ServiceComputePackageArgs, Mapping[str, Any]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">papertrails</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputePapertrailArgs, Mapping[str, Any], Awaitable[Union[ServiceComputePapertrailArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputePapertrailArgs, Mapping[str, Any], Awaitable[Union[ServiceComputePapertrailArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">s3loggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeS3loggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeS3loggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeS3loggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeS3loggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">splunks</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeSplunkArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSplunkArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeSplunkArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSplunkArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">sumologics</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeSumologicArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSumologicArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeSumologicArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSumologicArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">syslogs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeSyslogArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSyslogArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeSyslogArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSyslogArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">version_comment</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceCompute" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides a Fastly <a class="reference external" href="mailto:Compute&#37;&#52;&#48;Edge">Compute<span>&#64;</span>Edge</a> service. <a class="reference external" href="mailto:Compute&#37;&#52;&#48;Edge">Compute<span>&#64;</span>Edge</a> is a computation platform capable of running custom binaries that you compile on your own systems and upload to Fastly. Security and portability is provided by compiling your code to <a class="reference external" href="https://webassembly.org/">WebAssembly</a>, which is ran at the edge using <a class="reference external" href="https://github.com/bytecodealliance/lucet">Lucet</a>, an open-source WebAssembly runtime created by Fastly. A compute service encompasses Domains and Backends.</p>
<p>The Service resource requires a domain name that is correctly set up to direct
traffic to the Fastly service. See Fastly’s guide on [Adding CNAME Records][fastly-cname]
on their documentation site for guidance.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>activate</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to false. Default true.</p></li>
<li><p><strong>backends</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeBackendArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Backends to service requests from your Domains.
Defined below. Backends must be defined in this argument, or defined in the
<code class="docutils literal notranslate"><span class="pre">vcl</span></code> argument below</p></li>
<li><p><strong>bigqueryloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeBigqueryloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A BigQuery endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>blobstorageloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeBlobstorageloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An Azure Blob Storage endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>comment</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An optional comment about the Domain.</p></li>
<li><p><strong>domains</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeDomainArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – The domain of the DigitalOcean Spaces endpoint (default “nyc3.digitaloceanspaces.com”).</p></li>
<li><p><strong>force_destroy</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Services that are active cannot be destroyed. In
order to destroy the Service, set <code class="docutils literal notranslate"><span class="pre">force_destroy</span></code> to <code class="docutils literal notranslate"><span class="pre">true</span></code>. Default <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>gcsloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeGcsloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A gcs endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>healthchecks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeHealthcheckArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – Name of a defined <code class="docutils literal notranslate"><span class="pre">healthcheck</span></code> to assign to this backend.</p></li>
<li><p><strong>httpsloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeHttpsloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An HTTPS endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logentries</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLogentryArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A logentries endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>logging_cloudfiles</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingCloudfileArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Rackspace Cloud Files endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_datadogs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingDatadogArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Datadog endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_digitaloceans</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingDigitaloceanArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A DigitalOcean Spaces endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_elasticsearches</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingElasticsearchArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An Elasticsearch endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_ftps</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingFtpArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An FTP endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_googlepubsubs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingGooglepubsubArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Google Cloud Pub/Sub endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_heroku</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingHerokuArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Heroku endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_honeycombs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingHoneycombArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Honeycomb endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_kafkas</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingKafkaArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Kafka endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_logglies</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingLogglyArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Loggly endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_logshuttles</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingLogshuttleArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Log Shuttle endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_newrelics</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingNewrelicArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A New Relic endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_openstacks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingOpenstackArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An OpenStack endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_scalyrs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingScalyrArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Scalyr endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_sftps</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingSftpArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An SFTP endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique name of the Rackspace Cloud Files logging endpoint.</p></li>
<li><p><strong>package</strong> (<em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputePackageArgs'</em><em>]</em><em>]</em>) – A Wasm deployment package to upload. Defined below.</p></li>
<li><p><strong>papertrails</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputePapertrailArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Papertrail endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>s3loggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeS3loggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of S3 Buckets to send streaming logs too.
Defined below.</p></li>
<li><p><strong>splunks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeSplunkArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Splunk endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>sumologics</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeSumologicArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Sumologic endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>syslogs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeSyslogArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A syslog endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>version_comment</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Description field for the version.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">activate</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">active_version</span><span class="p">:</span> <span class="n">Union[float, Awaitable[float], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">backends</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeBackendArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBackendArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeBackendArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBackendArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">bigqueryloggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeBigqueryloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBigqueryloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeBigqueryloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBigqueryloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">blobstorageloggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeBlobstorageloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBlobstorageloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeBlobstorageloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeBlobstorageloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">cloned_version</span><span class="p">:</span> <span class="n">Union[float, Awaitable[float], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">comment</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">domains</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeDomainArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeDomainArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeDomainArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeDomainArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">force_destroy</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">gcsloggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeGcsloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeGcsloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeGcsloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeGcsloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">healthchecks</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeHealthcheckArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeHealthcheckArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeHealthcheckArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeHealthcheckArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">httpsloggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeHttpsloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeHttpsloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeHttpsloggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeHttpsloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logentries</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLogentryArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLogentryArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLogentryArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLogentryArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_cloudfiles</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingCloudfileArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingCloudfileArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingCloudfileArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingCloudfileArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_datadogs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingDatadogArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingDatadogArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingDatadogArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingDatadogArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_digitaloceans</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingDigitaloceanArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingDigitaloceanArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingDigitaloceanArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingDigitaloceanArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_elasticsearches</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingElasticsearchArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingElasticsearchArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingElasticsearchArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingElasticsearchArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_ftps</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingFtpArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingFtpArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingFtpArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingFtpArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_googlepubsubs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingGooglepubsubArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingGooglepubsubArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingGooglepubsubArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingGooglepubsubArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_heroku</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingHerokuArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingHerokuArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingHerokuArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingHerokuArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_honeycombs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingHoneycombArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingHoneycombArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingHoneycombArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingHoneycombArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_kafkas</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingKafkaArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingKafkaArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingKafkaArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingKafkaArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_logglies</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingLogglyArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingLogglyArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingLogglyArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingLogglyArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_logshuttles</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingLogshuttleArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingLogshuttleArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingLogshuttleArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingLogshuttleArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_newrelics</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingNewrelicArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingNewrelicArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingNewrelicArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingNewrelicArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_openstacks</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingOpenstackArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingOpenstackArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingOpenstackArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingOpenstackArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_scalyrs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingScalyrArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingScalyrArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingScalyrArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingScalyrArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_sftps</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeLoggingSftpArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingSftpArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeLoggingSftpArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeLoggingSftpArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">name</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">package</span><span class="p">:</span> <span class="n">Union[ServiceComputePackageArgs, Mapping[str, Any], Awaitable[Union[ServiceComputePackageArgs, Mapping[str, Any]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">papertrails</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputePapertrailArgs, Mapping[str, Any], Awaitable[Union[ServiceComputePapertrailArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputePapertrailArgs, Mapping[str, Any], Awaitable[Union[ServiceComputePapertrailArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">s3loggings</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeS3loggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeS3loggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeS3loggingArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeS3loggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">splunks</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeSplunkArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSplunkArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeSplunkArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSplunkArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">sumologics</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeSumologicArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSumologicArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeSumologicArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSumologicArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">syslogs</span><span class="p">:</span> <span class="n">Union[List[Union[ServiceComputeSyslogArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSyslogArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[ServiceComputeSyslogArgs, Mapping[str, Any], Awaitable[Union[ServiceComputeSyslogArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">version_comment</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_fastly.service_compute.ServiceCompute<a class="headerlink" href="#pulumi_fastly.ServiceCompute.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ServiceCompute resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>activate</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to false. Default true.</p></li>
<li><p><strong>active_version</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The currently active version of your Fastly Service.</p></li>
<li><p><strong>backends</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeBackendArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Backends to service requests from your Domains.
Defined below. Backends must be defined in this argument, or defined in the
<code class="docutils literal notranslate"><span class="pre">vcl</span></code> argument below</p></li>
<li><p><strong>bigqueryloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeBigqueryloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A BigQuery endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>blobstorageloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeBlobstorageloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An Azure Blob Storage endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>comment</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An optional comment about the Domain.</p></li>
<li><p><strong>domains</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeDomainArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – The domain of the DigitalOcean Spaces endpoint (default “nyc3.digitaloceanspaces.com”).</p></li>
<li><p><strong>force_destroy</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Services that are active cannot be destroyed. In
order to destroy the Service, set <code class="docutils literal notranslate"><span class="pre">force_destroy</span></code> to <code class="docutils literal notranslate"><span class="pre">true</span></code>. Default <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>gcsloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeGcsloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A gcs endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>healthchecks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeHealthcheckArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – Name of a defined <code class="docutils literal notranslate"><span class="pre">healthcheck</span></code> to assign to this backend.</p></li>
<li><p><strong>httpsloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeHttpsloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An HTTPS endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logentries</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLogentryArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A logentries endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>logging_cloudfiles</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingCloudfileArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Rackspace Cloud Files endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_datadogs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingDatadogArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Datadog endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_digitaloceans</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingDigitaloceanArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A DigitalOcean Spaces endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_elasticsearches</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingElasticsearchArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An Elasticsearch endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_ftps</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingFtpArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An FTP endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_googlepubsubs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingGooglepubsubArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Google Cloud Pub/Sub endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_heroku</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingHerokuArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Heroku endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_honeycombs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingHoneycombArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Honeycomb endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_kafkas</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingKafkaArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Kafka endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_logglies</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingLogglyArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Loggly endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_logshuttles</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingLogshuttleArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Log Shuttle endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_newrelics</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingNewrelicArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A New Relic endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_openstacks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingOpenstackArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An OpenStack endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_scalyrs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingScalyrArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Scalyr endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_sftps</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeLoggingSftpArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An SFTP endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique name of the Rackspace Cloud Files logging endpoint.</p></li>
<li><p><strong>package</strong> (<em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputePackageArgs'</em><em>]</em><em>]</em>) – A Wasm deployment package to upload. Defined below.</p></li>
<li><p><strong>papertrails</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputePapertrailArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Papertrail endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>s3loggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeS3loggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of S3 Buckets to send streaming logs too.
Defined below.</p></li>
<li><p><strong>splunks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeSplunkArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Splunk endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>sumologics</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeSumologicArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Sumologic endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>syslogs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'ServiceComputeSyslogArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A syslog endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>version_comment</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Description field for the version.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.activate">
<em class="property">property </em><code class="sig-name descname">activate</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.activate" title="Permalink to this definition">¶</a></dt>
<dd><p>Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to false. Default true.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.active_version">
<em class="property">property </em><code class="sig-name descname">active_version</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.active_version" title="Permalink to this definition">¶</a></dt>
<dd><p>The currently active version of your Fastly Service.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.backends">
<em class="property">property </em><code class="sig-name descname">backends</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.backends" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of Backends to service requests from your Domains.
Defined below. Backends must be defined in this argument, or defined in the
<code class="docutils literal notranslate"><span class="pre">vcl</span></code> argument below</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.bigqueryloggings">
<em class="property">property </em><code class="sig-name descname">bigqueryloggings</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.bigqueryloggings" title="Permalink to this definition">¶</a></dt>
<dd><p>A BigQuery endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.blobstorageloggings">
<em class="property">property </em><code class="sig-name descname">blobstorageloggings</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.blobstorageloggings" title="Permalink to this definition">¶</a></dt>
<dd><p>An Azure Blob Storage endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.comment">
<em class="property">property </em><code class="sig-name descname">comment</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.comment" title="Permalink to this definition">¶</a></dt>
<dd><p>An optional comment about the Domain.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.domains">
<em class="property">property </em><code class="sig-name descname">domains</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.domains" title="Permalink to this definition">¶</a></dt>
<dd><p>The domain of the DigitalOcean Spaces endpoint (default “nyc3.digitaloceanspaces.com”).</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.force_destroy">
<em class="property">property </em><code class="sig-name descname">force_destroy</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.force_destroy" title="Permalink to this definition">¶</a></dt>
<dd><p>Services that are active cannot be destroyed. In
order to destroy the Service, set <code class="docutils literal notranslate"><span class="pre">force_destroy</span></code> to <code class="docutils literal notranslate"><span class="pre">true</span></code>. Default <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.gcsloggings">
<em class="property">property </em><code class="sig-name descname">gcsloggings</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.gcsloggings" title="Permalink to this definition">¶</a></dt>
<dd><p>A gcs endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.healthchecks">
<em class="property">property </em><code class="sig-name descname">healthchecks</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.healthchecks" title="Permalink to this definition">¶</a></dt>
<dd><p>Name of a defined <code class="docutils literal notranslate"><span class="pre">healthcheck</span></code> to assign to this backend.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.httpsloggings">
<em class="property">property </em><code class="sig-name descname">httpsloggings</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.httpsloggings" title="Permalink to this definition">¶</a></dt>
<dd><p>An HTTPS endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logentries">
<em class="property">property </em><code class="sig-name descname">logentries</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logentries" title="Permalink to this definition">¶</a></dt>
<dd><p>A logentries endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_cloudfiles">
<em class="property">property </em><code class="sig-name descname">logging_cloudfiles</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_cloudfiles" title="Permalink to this definition">¶</a></dt>
<dd><p>A Rackspace Cloud Files endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_datadogs">
<em class="property">property </em><code class="sig-name descname">logging_datadogs</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_datadogs" title="Permalink to this definition">¶</a></dt>
<dd><p>A Datadog endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_digitaloceans">
<em class="property">property </em><code class="sig-name descname">logging_digitaloceans</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_digitaloceans" title="Permalink to this definition">¶</a></dt>
<dd><p>A DigitalOcean Spaces endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_elasticsearches">
<em class="property">property </em><code class="sig-name descname">logging_elasticsearches</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_elasticsearches" title="Permalink to this definition">¶</a></dt>
<dd><p>An Elasticsearch endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_ftps">
<em class="property">property </em><code class="sig-name descname">logging_ftps</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_ftps" title="Permalink to this definition">¶</a></dt>
<dd><p>An FTP endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_googlepubsubs">
<em class="property">property </em><code class="sig-name descname">logging_googlepubsubs</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_googlepubsubs" title="Permalink to this definition">¶</a></dt>
<dd><p>A Google Cloud Pub/Sub endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_heroku">
<em class="property">property </em><code class="sig-name descname">logging_heroku</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_heroku" title="Permalink to this definition">¶</a></dt>
<dd><p>A Heroku endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_honeycombs">
<em class="property">property </em><code class="sig-name descname">logging_honeycombs</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_honeycombs" title="Permalink to this definition">¶</a></dt>
<dd><p>A Honeycomb endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_kafkas">
<em class="property">property </em><code class="sig-name descname">logging_kafkas</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_kafkas" title="Permalink to this definition">¶</a></dt>
<dd><p>A Kafka endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_logglies">
<em class="property">property </em><code class="sig-name descname">logging_logglies</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_logglies" title="Permalink to this definition">¶</a></dt>
<dd><p>A Loggly endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_logshuttles">
<em class="property">property </em><code class="sig-name descname">logging_logshuttles</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_logshuttles" title="Permalink to this definition">¶</a></dt>
<dd><p>A Log Shuttle endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_newrelics">
<em class="property">property </em><code class="sig-name descname">logging_newrelics</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_newrelics" title="Permalink to this definition">¶</a></dt>
<dd><p>A New Relic endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_openstacks">
<em class="property">property </em><code class="sig-name descname">logging_openstacks</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_openstacks" title="Permalink to this definition">¶</a></dt>
<dd><p>An OpenStack endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_scalyrs">
<em class="property">property </em><code class="sig-name descname">logging_scalyrs</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_scalyrs" title="Permalink to this definition">¶</a></dt>
<dd><p>A Scalyr endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.logging_sftps">
<em class="property">property </em><code class="sig-name descname">logging_sftps</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.logging_sftps" title="Permalink to this definition">¶</a></dt>
<dd><p>An SFTP endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.name">
<em class="property">property </em><code class="sig-name descname">name</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The unique name of the Rackspace Cloud Files logging endpoint.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.package">
<em class="property">property </em><code class="sig-name descname">package</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.package" title="Permalink to this definition">¶</a></dt>
<dd><p>A Wasm deployment package to upload. Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.papertrails">
<em class="property">property </em><code class="sig-name descname">papertrails</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.papertrails" title="Permalink to this definition">¶</a></dt>
<dd><p>A Papertrail endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.s3loggings">
<em class="property">property </em><code class="sig-name descname">s3loggings</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.s3loggings" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of S3 Buckets to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.splunks">
<em class="property">property </em><code class="sig-name descname">splunks</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.splunks" title="Permalink to this definition">¶</a></dt>
<dd><p>A Splunk endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.sumologics">
<em class="property">property </em><code class="sig-name descname">sumologics</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.sumologics" title="Permalink to this definition">¶</a></dt>
<dd><p>A Sumologic endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.syslogs">
<em class="property">property </em><code class="sig-name descname">syslogs</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.syslogs" title="Permalink to this definition">¶</a></dt>
<dd><p>A syslog endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.version_comment">
<em class="property">property </em><code class="sig-name descname">version_comment</code><a class="headerlink" href="#pulumi_fastly.ServiceCompute.version_comment" title="Permalink to this definition">¶</a></dt>
<dd><p>Description field for the version.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceCompute.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceCompute.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceCompute.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_fastly.ServiceDictionaryItemsv1">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">ServiceDictionaryItemsv1</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">dictionary_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">items</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">service_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceDictionaryItemsv1" title="Permalink to this definition">¶</a></dt>
<dd><p>Defines a map of Fastly dictionary items that can be used to populate a service dictionary.  This resource will populate a dictionary with the items and will track their state.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">config</span> <span class="o">=</span> <span class="n">pulumi</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
<span class="n">mydict_name</span> <span class="o">=</span> <span class="n">config</span><span class="o">.</span><span class="n">get</span><span class="p">(</span><span class="s2">&quot;mydictName&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">mydict_name</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
    <span class="n">mydict_name</span> <span class="o">=</span> <span class="s2">&quot;My Dictionary&quot;</span>
<span class="n">myservice</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1</span><span class="p">(</span><span class="s2">&quot;myservice&quot;</span><span class="p">,</span>
    <span class="n">domains</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DomainArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com&quot;</span><span class="p">,</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">backends</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
        <span class="n">address</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com.s3-website-us-west-2.amazonaws.com&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;AWS S3 hosting&quot;</span><span class="p">,</span>
        <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">dictionaries</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DictionaryArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="n">mydict_name</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">force_destroy</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">items</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">ServiceDictionaryItemsv1</span><span class="p">(</span><span class="s2">&quot;items&quot;</span><span class="p">,</span>
    <span class="n">service_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">id</span><span class="p">,</span>
    <span class="n">dictionary_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">dictionaries</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="n">dictionaries</span><span class="p">:</span> <span class="p">{</span><span class="n">s</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">s</span><span class="o">.</span><span class="n">dictionary_id</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">dictionaries</span><span class="p">}[</span><span class="n">mydict_name</span><span class="p">]),</span>
    <span class="n">items</span><span class="o">=</span><span class="p">{</span>
        <span class="s2">&quot;key1&quot;</span><span class="p">:</span> <span class="s2">&quot;value1&quot;</span><span class="p">,</span>
        <span class="s2">&quot;key2&quot;</span><span class="p">:</span> <span class="s2">&quot;value2&quot;</span><span class="p">,</span>
    <span class="p">})</span>
</pre></div>
</div>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">config</span> <span class="o">=</span> <span class="n">pulumi</span><span class="o">.</span><span class="n">Config</span><span class="p">()</span>
<span class="n">mydict</span> <span class="o">=</span> <span class="n">config</span><span class="o">.</span><span class="n">get_object</span><span class="p">(</span><span class="s2">&quot;mydict&quot;</span><span class="p">)</span>
<span class="k">if</span> <span class="n">mydict</span> <span class="ow">is</span> <span class="kc">None</span><span class="p">:</span>
    <span class="n">mydict</span> <span class="o">=</span> <span class="p">{</span>
        <span class="s2">&quot;name&quot;</span><span class="p">:</span> <span class="s2">&quot;My Dictionary&quot;</span><span class="p">,</span>
        <span class="s2">&quot;items&quot;</span><span class="p">:</span> <span class="p">{</span>
            <span class="s2">&quot;key1&quot;</span><span class="p">:</span> <span class="s2">&quot;value1x&quot;</span><span class="p">,</span>
            <span class="s2">&quot;key2&quot;</span><span class="p">:</span> <span class="s2">&quot;value2x&quot;</span><span class="p">,</span>
        <span class="p">},</span>
    <span class="p">}</span>
<span class="n">myservice</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1</span><span class="p">(</span><span class="s2">&quot;myservice&quot;</span><span class="p">,</span>
    <span class="n">domains</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DomainArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com&quot;</span><span class="p">,</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">backends</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
        <span class="n">address</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com.s3-website-us-west-2.amazonaws.com&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;AWS S3 hosting&quot;</span><span class="p">,</span>
        <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">dictionaries</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DictionaryArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="n">mydict</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">],</span>
    <span class="p">)],</span>
    <span class="n">force_destroy</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">items</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">ServiceDictionaryItemsv1</span><span class="p">(</span><span class="s2">&quot;items&quot;</span><span class="p">,</span>
    <span class="n">service_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">id</span><span class="p">,</span>
    <span class="n">dictionary_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">dictionaries</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="n">dictionaries</span><span class="p">:</span> <span class="p">{</span><span class="n">d</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">d</span><span class="o">.</span><span class="n">dictionary_id</span> <span class="k">for</span> <span class="n">d</span> <span class="ow">in</span> <span class="n">dictionaries</span><span class="p">}[</span><span class="n">mydict</span><span class="p">[</span><span class="s2">&quot;name&quot;</span><span class="p">]]),</span>
    <span class="n">items</span><span class="o">=</span><span class="n">mydict</span><span class="p">[</span><span class="s2">&quot;items&quot;</span><span class="p">])</span>
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>dictionary_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the dictionary that the items belong to</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>items</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – A map representing an entry in the dictionary, (key/value)</p></li>
<li><p><strong>service_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the service that the dictionary belongs to</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_fastly.ServiceDictionaryItemsv1.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">dictionary_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">items</span><span class="p">:</span> <span class="n">Union[Mapping[str, Any], Awaitable[Mapping[str, Any]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">service_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_fastly.service_dictionary_itemsv1.ServiceDictionaryItemsv1<a class="headerlink" href="#pulumi_fastly.ServiceDictionaryItemsv1.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ServiceDictionaryItemsv1 resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>dictionary_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the dictionary that the items belong to</p></li>
<li><p><strong>Any</strong><strong>]</strong><strong>] </strong><strong>items</strong> (<em>pulumi.Input</em><em>[</em><em>Mapping</em><em>[</em><em>str</em><em>,</em>) – A map representing an entry in the dictionary, (key/value)</p></li>
<li><p><strong>service_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the service that the dictionary belongs to</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDictionaryItemsv1.dictionary_id">
<em class="property">property </em><code class="sig-name descname">dictionary_id</code><a class="headerlink" href="#pulumi_fastly.ServiceDictionaryItemsv1.dictionary_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the dictionary that the items belong to</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDictionaryItemsv1.items">
<em class="property">property </em><code class="sig-name descname">items</code><a class="headerlink" href="#pulumi_fastly.ServiceDictionaryItemsv1.items" title="Permalink to this definition">¶</a></dt>
<dd><p>A map representing an entry in the dictionary, (key/value)</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDictionaryItemsv1.service_id">
<em class="property">property </em><code class="sig-name descname">service_id</code><a class="headerlink" href="#pulumi_fastly.ServiceDictionaryItemsv1.service_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the service that the dictionary belongs to</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDictionaryItemsv1.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceDictionaryItemsv1.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDictionaryItemsv1.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceDictionaryItemsv1.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_fastly.ServiceDynamicSnippetContentv1">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">ServiceDynamicSnippetContentv1</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">content</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">service_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">snippet_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceDynamicSnippetContentv1" title="Permalink to this definition">¶</a></dt>
<dd><p>Defines content that represents blocks of VCL logic that is inserted into your service.  This resource will populate the content of a dynamic snippet and allow it to be manged without the creation of a new service verison.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">myservice</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1</span><span class="p">(</span><span class="s2">&quot;myservice&quot;</span><span class="p">,</span>
    <span class="n">domains</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DomainArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;snippet.fastlytestdomain.com&quot;</span><span class="p">,</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;snippet test&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">backends</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
        <span class="n">address</span><span class="o">=</span><span class="s2">&quot;tftesting.tftesting.net.s3-website-us-west-2.amazonaws.com&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;AWS S3 hosting&quot;</span><span class="p">,</span>
        <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">dynamicsnippets</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DynamicsnippetArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;My Dynamic Snippet&quot;</span><span class="p">,</span>
        <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;recv&quot;</span><span class="p">,</span>
        <span class="n">priority</span><span class="o">=</span><span class="mi">110</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">default_host</span><span class="o">=</span><span class="s2">&quot;tftesting.tftesting.net.s3-website-us-west-2.amazonaws.com&quot;</span><span class="p">,</span>
    <span class="n">force_destroy</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">my_dyn_content</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">ServiceDynamicSnippetContentv1</span><span class="p">(</span><span class="s2">&quot;myDynContent&quot;</span><span class="p">,</span>
    <span class="n">service_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">id</span><span class="p">,</span>
    <span class="n">snippet_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">dynamicsnippets</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="n">dynamicsnippets</span><span class="p">:</span> <span class="p">{</span><span class="n">s</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">s</span><span class="o">.</span><span class="n">snippet_id</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">dynamicsnippets</span><span class="p">}[</span><span class="s2">&quot;My Dynamic Snippet&quot;</span><span class="p">]),</span>
    <span class="n">content</span><span class="o">=</span><span class="s2">&quot;&quot;&quot;if ( req.url ) {</span>
<span class="s2"> set req.http.my-snippet-test-header = &quot;true&quot;;</span>
<span class="s2">}&quot;&quot;&quot;</span><span class="p">)</span>
</pre></div>
</div>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">myservice</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1</span><span class="p">(</span><span class="s2">&quot;myservice&quot;</span><span class="p">,</span>
    <span class="n">domains</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DomainArgs</span><span class="p">(</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;snippet.fastlytestdomain.com&quot;</span><span class="p">,</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;snippet test&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">backends</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
        <span class="n">address</span><span class="o">=</span><span class="s2">&quot;tftesting.tftesting.net.s3-website-us-west-2.amazonaws.com&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;AWS S3 hosting&quot;</span><span class="p">,</span>
        <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">dynamicsnippets</span><span class="o">=</span><span class="p">[</span>
        <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DynamicsnippetArgs</span><span class="p">(</span>
            <span class="n">name</span><span class="o">=</span><span class="s2">&quot;My Dynamic Snippet One&quot;</span><span class="p">,</span>
            <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;recv&quot;</span><span class="p">,</span>
            <span class="n">priority</span><span class="o">=</span><span class="mi">110</span><span class="p">,</span>
        <span class="p">),</span>
        <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DynamicsnippetArgs</span><span class="p">(</span>
            <span class="n">name</span><span class="o">=</span><span class="s2">&quot;My Dynamic Snippet Two&quot;</span><span class="p">,</span>
            <span class="nb">type</span><span class="o">=</span><span class="s2">&quot;recv&quot;</span><span class="p">,</span>
            <span class="n">priority</span><span class="o">=</span><span class="mi">110</span><span class="p">,</span>
        <span class="p">),</span>
    <span class="p">],</span>
    <span class="n">default_host</span><span class="o">=</span><span class="s2">&quot;tftesting.tftesting.net.s3-website-us-west-2.amazonaws.com&quot;</span><span class="p">,</span>
    <span class="n">force_destroy</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
<span class="n">my_dyn_content_one</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">ServiceDynamicSnippetContentv1</span><span class="p">(</span><span class="s2">&quot;myDynContentOne&quot;</span><span class="p">,</span>
    <span class="n">service_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">id</span><span class="p">,</span>
    <span class="n">snippet_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">dynamicsnippets</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="n">dynamicsnippets</span><span class="p">:</span> <span class="p">{</span><span class="n">s</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">s</span><span class="o">.</span><span class="n">snippet_id</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">dynamicsnippets</span><span class="p">}[</span><span class="s2">&quot;My Dynamic Snippet One&quot;</span><span class="p">]),</span>
    <span class="n">content</span><span class="o">=</span><span class="s2">&quot;&quot;&quot;if ( req.url ) {</span>
<span class="s2"> set req.http.my-snippet-test-header-one = &quot;true&quot;;</span>
<span class="s2">}&quot;&quot;&quot;</span><span class="p">)</span>
<span class="n">my_dyn_content_two</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">ServiceDynamicSnippetContentv1</span><span class="p">(</span><span class="s2">&quot;myDynContentTwo&quot;</span><span class="p">,</span>
    <span class="n">service_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">id</span><span class="p">,</span>
    <span class="n">snippet_id</span><span class="o">=</span><span class="n">myservice</span><span class="o">.</span><span class="n">dynamicsnippets</span><span class="o">.</span><span class="n">apply</span><span class="p">(</span><span class="k">lambda</span> <span class="n">dynamicsnippets</span><span class="p">:</span> <span class="p">{</span><span class="n">s</span><span class="o">.</span><span class="n">name</span><span class="p">:</span> <span class="n">s</span><span class="o">.</span><span class="n">snippet_id</span> <span class="k">for</span> <span class="n">s</span> <span class="ow">in</span> <span class="n">dynamicsnippets</span><span class="p">}[</span><span class="s2">&quot;My Dynamic Snippet Two&quot;</span><span class="p">]),</span>
    <span class="n">content</span><span class="o">=</span><span class="s2">&quot;&quot;&quot;if ( req.url ) {</span>
<span class="s2"> set req.http.my-snippet-test-header-two = &quot;true&quot;;</span>
<span class="s2">}&quot;&quot;&quot;</span><span class="p">)</span>
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>content</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The VCL code that specifies exactly what the snippet does.</p></li>
<li><p><strong>service_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the service that the dynamic snippet belongs to</p></li>
<li><p><strong>snippet_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the dynamic snippet that the content belong to</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_fastly.ServiceDynamicSnippetContentv1.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">content</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">service_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">snippet_id</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_fastly.service_dynamic_snippet_contentv1.ServiceDynamicSnippetContentv1<a class="headerlink" href="#pulumi_fastly.ServiceDynamicSnippetContentv1.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing ServiceDynamicSnippetContentv1 resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>content</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The VCL code that specifies exactly what the snippet does.</p></li>
<li><p><strong>service_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the service that the dynamic snippet belongs to</p></li>
<li><p><strong>snippet_id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The ID of the dynamic snippet that the content belong to</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDynamicSnippetContentv1.content">
<em class="property">property </em><code class="sig-name descname">content</code><a class="headerlink" href="#pulumi_fastly.ServiceDynamicSnippetContentv1.content" title="Permalink to this definition">¶</a></dt>
<dd><p>The VCL code that specifies exactly what the snippet does.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDynamicSnippetContentv1.service_id">
<em class="property">property </em><code class="sig-name descname">service_id</code><a class="headerlink" href="#pulumi_fastly.ServiceDynamicSnippetContentv1.service_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the service that the dynamic snippet belongs to</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDynamicSnippetContentv1.snippet_id">
<em class="property">property </em><code class="sig-name descname">snippet_id</code><a class="headerlink" href="#pulumi_fastly.ServiceDynamicSnippetContentv1.snippet_id" title="Permalink to this definition">¶</a></dt>
<dd><p>The ID of the dynamic snippet that the content belong to</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDynamicSnippetContentv1.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceDynamicSnippetContentv1.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.ServiceDynamicSnippetContentv1.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.ServiceDynamicSnippetContentv1.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_fastly.Servicev1">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">Servicev1</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">acls</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1AclArgs, Mapping[str, Any], Awaitable[Union[Servicev1AclArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1AclArgs, Mapping[str, Any], Awaitable[Union[Servicev1AclArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">activate</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">backends</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1BackendArgs, Mapping[str, Any], Awaitable[Union[Servicev1BackendArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1BackendArgs, Mapping[str, Any], Awaitable[Union[Servicev1BackendArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">bigqueryloggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1BigqueryloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1BigqueryloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1BigqueryloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1BigqueryloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">blobstorageloggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1BlobstorageloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1BlobstorageloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1BlobstorageloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1BlobstorageloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">cache_settings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1CacheSettingArgs, Mapping[str, Any], Awaitable[Union[Servicev1CacheSettingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1CacheSettingArgs, Mapping[str, Any], Awaitable[Union[Servicev1CacheSettingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">comment</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">conditions</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1ConditionArgs, Mapping[str, Any], Awaitable[Union[Servicev1ConditionArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1ConditionArgs, Mapping[str, Any], Awaitable[Union[Servicev1ConditionArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">default_host</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">default_ttl</span><span class="p">:</span> <span class="n">Union[float, Awaitable[float], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">dictionaries</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1DictionaryArgs, Mapping[str, Any], Awaitable[Union[Servicev1DictionaryArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1DictionaryArgs, Mapping[str, Any], Awaitable[Union[Servicev1DictionaryArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">directors</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1DirectorArgs, Mapping[str, Any], Awaitable[Union[Servicev1DirectorArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1DirectorArgs, Mapping[str, Any], Awaitable[Union[Servicev1DirectorArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">domains</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1DomainArgs, Mapping[str, Any], Awaitable[Union[Servicev1DomainArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1DomainArgs, Mapping[str, Any], Awaitable[Union[Servicev1DomainArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">dynamicsnippets</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1DynamicsnippetArgs, Mapping[str, Any], Awaitable[Union[Servicev1DynamicsnippetArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1DynamicsnippetArgs, Mapping[str, Any], Awaitable[Union[Servicev1DynamicsnippetArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">force_destroy</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">gcsloggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1GcsloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1GcsloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1GcsloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1GcsloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">gzips</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1GzipArgs, Mapping[str, Any], Awaitable[Union[Servicev1GzipArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1GzipArgs, Mapping[str, Any], Awaitable[Union[Servicev1GzipArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">headers</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1HeaderArgs, Mapping[str, Any], Awaitable[Union[Servicev1HeaderArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1HeaderArgs, Mapping[str, Any], Awaitable[Union[Servicev1HeaderArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">healthchecks</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1HealthcheckArgs, Mapping[str, Any], Awaitable[Union[Servicev1HealthcheckArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1HealthcheckArgs, Mapping[str, Any], Awaitable[Union[Servicev1HealthcheckArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">httpsloggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1HttpsloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1HttpsloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1HttpsloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1HttpsloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logentries</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LogentryArgs, Mapping[str, Any], Awaitable[Union[Servicev1LogentryArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LogentryArgs, Mapping[str, Any], Awaitable[Union[Servicev1LogentryArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_cloudfiles</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingCloudfileArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingCloudfileArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingCloudfileArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingCloudfileArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_datadogs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingDatadogArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingDatadogArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingDatadogArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingDatadogArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_digitaloceans</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingDigitaloceanArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingDigitaloceanArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingDigitaloceanArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingDigitaloceanArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_elasticsearches</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingElasticsearchArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingElasticsearchArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingElasticsearchArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingElasticsearchArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_ftps</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingFtpArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingFtpArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingFtpArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingFtpArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_googlepubsubs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingGooglepubsubArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingGooglepubsubArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingGooglepubsubArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingGooglepubsubArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_heroku</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingHerokuArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingHerokuArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingHerokuArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingHerokuArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_honeycombs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingHoneycombArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingHoneycombArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingHoneycombArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingHoneycombArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_kafkas</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingKafkaArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingKafkaArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingKafkaArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingKafkaArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_logglies</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingLogglyArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingLogglyArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingLogglyArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingLogglyArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_logshuttles</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingLogshuttleArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingLogshuttleArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingLogshuttleArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingLogshuttleArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_newrelics</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingNewrelicArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingNewrelicArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingNewrelicArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingNewrelicArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_openstacks</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingOpenstackArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingOpenstackArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingOpenstackArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingOpenstackArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_scalyrs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingScalyrArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingScalyrArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingScalyrArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingScalyrArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_sftps</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingSftpArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingSftpArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingSftpArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingSftpArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">name</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">papertrails</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1PapertrailArgs, Mapping[str, Any], Awaitable[Union[Servicev1PapertrailArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1PapertrailArgs, Mapping[str, Any], Awaitable[Union[Servicev1PapertrailArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">request_settings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1RequestSettingArgs, Mapping[str, Any], Awaitable[Union[Servicev1RequestSettingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1RequestSettingArgs, Mapping[str, Any], Awaitable[Union[Servicev1RequestSettingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">response_objects</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1ResponseObjectArgs, Mapping[str, Any], Awaitable[Union[Servicev1ResponseObjectArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1ResponseObjectArgs, Mapping[str, Any], Awaitable[Union[Servicev1ResponseObjectArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">s3loggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1S3loggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1S3loggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1S3loggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1S3loggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">snippets</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1SnippetArgs, Mapping[str, Any], Awaitable[Union[Servicev1SnippetArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1SnippetArgs, Mapping[str, Any], Awaitable[Union[Servicev1SnippetArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">splunks</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1SplunkArgs, Mapping[str, Any], Awaitable[Union[Servicev1SplunkArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1SplunkArgs, Mapping[str, Any], Awaitable[Union[Servicev1SplunkArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">sumologics</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1SumologicArgs, Mapping[str, Any], Awaitable[Union[Servicev1SumologicArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1SumologicArgs, Mapping[str, Any], Awaitable[Union[Servicev1SumologicArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">syslogs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1SyslogArgs, Mapping[str, Any], Awaitable[Union[Servicev1SyslogArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1SyslogArgs, Mapping[str, Any], Awaitable[Union[Servicev1SyslogArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">vcls</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1VclArgs, Mapping[str, Any], Awaitable[Union[Servicev1VclArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1VclArgs, Mapping[str, Any], Awaitable[Union[Servicev1VclArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">version_comment</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Servicev1" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides a Fastly Service, representing the configuration for a website, app,
API, or anything else to be served through Fastly. A Service encompasses Domains
and Backends.</p>
<p>The Service resource requires a domain name that is correctly set up to direct
traffic to the Fastly service. See Fastly’s guide on [Adding CNAME Records][fastly-cname]
on their documentation site for guidance.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">demo</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1</span><span class="p">(</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
    <span class="n">backends</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
        <span class="n">address</span><span class="o">=</span><span class="s2">&quot;127.0.0.1&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;localhost&quot;</span><span class="p">,</span>
        <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">domains</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DomainArgs</span><span class="p">(</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">force_destroy</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
</pre></div>
</div>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">demo</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1</span><span class="p">(</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
    <span class="n">backends</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
        <span class="n">address</span><span class="o">=</span><span class="s2">&quot;127.0.0.1&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;localhost&quot;</span><span class="p">,</span>
        <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">domains</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DomainArgs</span><span class="p">(</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">force_destroy</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
    <span class="n">vcls</span><span class="o">=</span><span class="p">[</span>
        <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1VclArgs</span><span class="p">(</span>
            <span class="n">content</span><span class="o">=</span><span class="p">(</span><span class="k">lambda</span> <span class="n">path</span><span class="p">:</span> <span class="nb">open</span><span class="p">(</span><span class="n">path</span><span class="p">)</span><span class="o">.</span><span class="n">read</span><span class="p">())(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">path</span><span class="p">[</span><span class="s1">&#39;module&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">/my_custom_main.vcl&quot;</span><span class="p">),</span>
            <span class="n">main</span><span class="o">=</span><span class="kc">True</span><span class="p">,</span>
            <span class="n">name</span><span class="o">=</span><span class="s2">&quot;my_custom_main_vcl&quot;</span><span class="p">,</span>
        <span class="p">),</span>
        <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1VclArgs</span><span class="p">(</span>
            <span class="n">content</span><span class="o">=</span><span class="p">(</span><span class="k">lambda</span> <span class="n">path</span><span class="p">:</span> <span class="nb">open</span><span class="p">(</span><span class="n">path</span><span class="p">)</span><span class="o">.</span><span class="n">read</span><span class="p">())(</span><span class="sa">f</span><span class="s2">&quot;</span><span class="si">{</span><span class="n">path</span><span class="p">[</span><span class="s1">&#39;module&#39;</span><span class="p">]</span><span class="si">}</span><span class="s2">/my_custom_library.vcl&quot;</span><span class="p">),</span>
            <span class="n">name</span><span class="o">=</span><span class="s2">&quot;my_custom_library_vcl&quot;</span><span class="p">,</span>
        <span class="p">),</span>
    <span class="p">])</span>
</pre></div>
</div>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">demo</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1</span><span class="p">(</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
    <span class="n">backends</span><span class="o">=</span><span class="p">[</span>
        <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
            <span class="n">address</span><span class="o">=</span><span class="s2">&quot;127.0.0.1&quot;</span><span class="p">,</span>
            <span class="n">name</span><span class="o">=</span><span class="s2">&quot;origin1&quot;</span><span class="p">,</span>
            <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
        <span class="p">),</span>
        <span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1BackendArgs</span><span class="p">(</span>
            <span class="n">address</span><span class="o">=</span><span class="s2">&quot;127.0.0.2&quot;</span><span class="p">,</span>
            <span class="n">name</span><span class="o">=</span><span class="s2">&quot;origin2&quot;</span><span class="p">,</span>
            <span class="n">port</span><span class="o">=</span><span class="mi">80</span><span class="p">,</span>
        <span class="p">),</span>
    <span class="p">],</span>
    <span class="n">directors</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DirectorArgs</span><span class="p">(</span>
        <span class="n">backends</span><span class="o">=</span><span class="p">[</span>
            <span class="s2">&quot;origin1&quot;</span><span class="p">,</span>
            <span class="s2">&quot;origin2&quot;</span><span class="p">,</span>
        <span class="p">],</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;mydirector&quot;</span><span class="p">,</span>
        <span class="n">quorum</span><span class="o">=</span><span class="mi">0</span><span class="p">,</span>
        <span class="nb">type</span><span class="o">=</span><span class="mi">3</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">domains</span><span class="o">=</span><span class="p">[</span><span class="n">fastly</span><span class="o">.</span><span class="n">Servicev1DomainArgs</span><span class="p">(</span>
        <span class="n">comment</span><span class="o">=</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span>
        <span class="n">name</span><span class="o">=</span><span class="s2">&quot;demo.notexample.com&quot;</span><span class="p">,</span>
    <span class="p">)],</span>
    <span class="n">force_destroy</span><span class="o">=</span><span class="kc">True</span><span class="p">)</span>
</pre></div>
</div>
<blockquote>
<div><p><strong>Note:</strong> For an AWS S3 Bucket, the Backend address is
<code class="docutils literal notranslate"><span class="pre">&lt;domain&gt;.s3-website-&lt;region&gt;.amazonaws.com</span></code>. The <code class="docutils literal notranslate"><span class="pre">default_host</span></code> attribute
should be set to <code class="docutils literal notranslate"><span class="pre">&lt;bucket_name&gt;.s3-website-&lt;region&gt;.amazonaws.com</span></code>. See the
Fastly documentation on [Amazon S3][fastly-s3].</p>
</div></blockquote>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>acls</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1AclArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of ACL configuration blocks.  Defined below.</p></li>
<li><p><strong>activate</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to false. Default true.</p></li>
<li><p><strong>backends</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1BackendArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Backends to service requests from your Domains.
Defined below. Backends must be defined in this argument, or defined in the
<code class="docutils literal notranslate"><span class="pre">vcl</span></code> argument below</p></li>
<li><p><strong>bigqueryloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1BigqueryloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A BigQuery endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>blobstorageloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1BlobstorageloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An Azure Blob Storage endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>cache_settings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1CacheSettingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Cache Settings, allowing you to override</p></li>
<li><p><strong>comment</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An optional comment about the Director.</p></li>
<li><p><strong>conditions</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1ConditionArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of conditions to add logic to any basic
configuration object in this service. Defined below.</p></li>
<li><p><strong>default_host</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Sets the host header.</p></li>
<li><p><strong>default_ttl</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The default Time-to-live (TTL) for
requests.</p></li>
<li><p><strong>dictionaries</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1DictionaryArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of dictionaries that allow the storing of key values pair for use within VCL functions. Defined below.</p></li>
<li><p><strong>directors</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1DirectorArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A director to allow more control over balancing traffic over backends.
when an item is not to be cached based on an above <code class="docutils literal notranslate"><span class="pre">condition</span></code>. Defined below</p></li>
<li><p><strong>domains</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1DomainArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – The domain of the DigitalOcean Spaces endpoint (default “nyc3.digitaloceanspaces.com”).</p></li>
<li><p><strong>dynamicsnippets</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1DynamicsnippetArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of custom, “dynamic” VCL Snippet configuration blocks.  Defined below.</p></li>
<li><p><strong>force_destroy</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Services that are active cannot be destroyed. In
order to destroy the Service, set <code class="docutils literal notranslate"><span class="pre">force_destroy</span></code> to <code class="docutils literal notranslate"><span class="pre">true</span></code>. Default <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>gcsloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1GcsloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A gcs endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>gzips</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1GzipArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of gzip rules to control automatic gzipping of
content. Defined below.</p></li>
<li><p><strong>headers</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1HeaderArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Headers to manipulate for each request. Defined
below.</p></li>
<li><p><strong>healthchecks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1HealthcheckArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – Name of a defined <code class="docutils literal notranslate"><span class="pre">healthcheck</span></code> to assign to this backend.</p></li>
<li><p><strong>httpsloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1HttpsloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An HTTPS endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logentries</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LogentryArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A logentries endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>logging_cloudfiles</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingCloudfileArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Rackspace Cloud Files endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_datadogs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingDatadogArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Datadog endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_digitaloceans</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingDigitaloceanArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A DigitalOcean Spaces endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_elasticsearches</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingElasticsearchArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An Elasticsearch endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_ftps</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingFtpArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An FTP endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_googlepubsubs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingGooglepubsubArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Google Cloud Pub/Sub endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_heroku</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingHerokuArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Heroku endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_honeycombs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingHoneycombArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Honeycomb endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_kafkas</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingKafkaArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Kafka endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_logglies</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingLogglyArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Loggly endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_logshuttles</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingLogshuttleArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Log Shuttle endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_newrelics</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingNewrelicArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A New Relic endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_openstacks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingOpenstackArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An OpenStack endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_scalyrs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingScalyrArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Scalyr endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_sftps</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingSftpArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An SFTP endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A unique name to identify this dictionary.</p></li>
<li><p><strong>papertrails</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1PapertrailArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Papertrail endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>request_settings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1RequestSettingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Request modifiers. Defined below</p></li>
<li><p><strong>response_objects</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1ResponseObjectArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – Allows you to create synthetic responses that exist entirely on the varnish machine. Useful for creating error or maintenance pages that exists outside the scope of your datacenter. Best when used with Condition objects.</p></li>
<li><p><strong>s3loggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1S3loggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of S3 Buckets to send streaming logs too.
Defined below.</p></li>
<li><p><strong>snippets</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1SnippetArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of custom, “regular” (non-dynamic) VCL Snippet configuration blocks.  Defined below.</p></li>
<li><p><strong>splunks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1SplunkArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Splunk endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>sumologics</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1SumologicArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Sumologic endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>syslogs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1SyslogArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A syslog endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>vcls</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1VclArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of custom VCL configuration blocks. See the <a class="reference external" href="https://docs.fastly.com/vcl/custom-vcl/uploading-custom-vcl/">Fastly documentation</a> for more information on using custom VCL.</p></li>
<li><p><strong>version_comment</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Description field for the version.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_fastly.Servicev1.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">acls</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1AclArgs, Mapping[str, Any], Awaitable[Union[Servicev1AclArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1AclArgs, Mapping[str, Any], Awaitable[Union[Servicev1AclArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">activate</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">active_version</span><span class="p">:</span> <span class="n">Union[float, Awaitable[float], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">backends</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1BackendArgs, Mapping[str, Any], Awaitable[Union[Servicev1BackendArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1BackendArgs, Mapping[str, Any], Awaitable[Union[Servicev1BackendArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">bigqueryloggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1BigqueryloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1BigqueryloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1BigqueryloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1BigqueryloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">blobstorageloggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1BlobstorageloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1BlobstorageloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1BlobstorageloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1BlobstorageloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">cache_settings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1CacheSettingArgs, Mapping[str, Any], Awaitable[Union[Servicev1CacheSettingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1CacheSettingArgs, Mapping[str, Any], Awaitable[Union[Servicev1CacheSettingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">cloned_version</span><span class="p">:</span> <span class="n">Union[float, Awaitable[float], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">comment</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">conditions</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1ConditionArgs, Mapping[str, Any], Awaitable[Union[Servicev1ConditionArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1ConditionArgs, Mapping[str, Any], Awaitable[Union[Servicev1ConditionArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">default_host</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">default_ttl</span><span class="p">:</span> <span class="n">Union[float, Awaitable[float], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">dictionaries</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1DictionaryArgs, Mapping[str, Any], Awaitable[Union[Servicev1DictionaryArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1DictionaryArgs, Mapping[str, Any], Awaitable[Union[Servicev1DictionaryArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">directors</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1DirectorArgs, Mapping[str, Any], Awaitable[Union[Servicev1DirectorArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1DirectorArgs, Mapping[str, Any], Awaitable[Union[Servicev1DirectorArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">domains</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1DomainArgs, Mapping[str, Any], Awaitable[Union[Servicev1DomainArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1DomainArgs, Mapping[str, Any], Awaitable[Union[Servicev1DomainArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">dynamicsnippets</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1DynamicsnippetArgs, Mapping[str, Any], Awaitable[Union[Servicev1DynamicsnippetArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1DynamicsnippetArgs, Mapping[str, Any], Awaitable[Union[Servicev1DynamicsnippetArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">force_destroy</span><span class="p">:</span> <span class="n">Union[bool, Awaitable[bool], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">gcsloggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1GcsloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1GcsloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1GcsloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1GcsloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">gzips</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1GzipArgs, Mapping[str, Any], Awaitable[Union[Servicev1GzipArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1GzipArgs, Mapping[str, Any], Awaitable[Union[Servicev1GzipArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">headers</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1HeaderArgs, Mapping[str, Any], Awaitable[Union[Servicev1HeaderArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1HeaderArgs, Mapping[str, Any], Awaitable[Union[Servicev1HeaderArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">healthchecks</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1HealthcheckArgs, Mapping[str, Any], Awaitable[Union[Servicev1HealthcheckArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1HealthcheckArgs, Mapping[str, Any], Awaitable[Union[Servicev1HealthcheckArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">httpsloggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1HttpsloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1HttpsloggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1HttpsloggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1HttpsloggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logentries</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LogentryArgs, Mapping[str, Any], Awaitable[Union[Servicev1LogentryArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LogentryArgs, Mapping[str, Any], Awaitable[Union[Servicev1LogentryArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_cloudfiles</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingCloudfileArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingCloudfileArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingCloudfileArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingCloudfileArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_datadogs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingDatadogArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingDatadogArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingDatadogArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingDatadogArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_digitaloceans</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingDigitaloceanArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingDigitaloceanArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingDigitaloceanArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingDigitaloceanArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_elasticsearches</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingElasticsearchArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingElasticsearchArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingElasticsearchArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingElasticsearchArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_ftps</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingFtpArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingFtpArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingFtpArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingFtpArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_googlepubsubs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingGooglepubsubArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingGooglepubsubArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingGooglepubsubArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingGooglepubsubArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_heroku</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingHerokuArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingHerokuArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingHerokuArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingHerokuArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_honeycombs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingHoneycombArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingHoneycombArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingHoneycombArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingHoneycombArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_kafkas</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingKafkaArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingKafkaArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingKafkaArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingKafkaArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_logglies</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingLogglyArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingLogglyArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingLogglyArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingLogglyArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_logshuttles</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingLogshuttleArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingLogshuttleArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingLogshuttleArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingLogshuttleArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_newrelics</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingNewrelicArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingNewrelicArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingNewrelicArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingNewrelicArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_openstacks</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingOpenstackArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingOpenstackArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingOpenstackArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingOpenstackArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_scalyrs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingScalyrArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingScalyrArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingScalyrArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingScalyrArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">logging_sftps</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1LoggingSftpArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingSftpArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1LoggingSftpArgs, Mapping[str, Any], Awaitable[Union[Servicev1LoggingSftpArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">name</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">papertrails</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1PapertrailArgs, Mapping[str, Any], Awaitable[Union[Servicev1PapertrailArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1PapertrailArgs, Mapping[str, Any], Awaitable[Union[Servicev1PapertrailArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">request_settings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1RequestSettingArgs, Mapping[str, Any], Awaitable[Union[Servicev1RequestSettingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1RequestSettingArgs, Mapping[str, Any], Awaitable[Union[Servicev1RequestSettingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">response_objects</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1ResponseObjectArgs, Mapping[str, Any], Awaitable[Union[Servicev1ResponseObjectArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1ResponseObjectArgs, Mapping[str, Any], Awaitable[Union[Servicev1ResponseObjectArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">s3loggings</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1S3loggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1S3loggingArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1S3loggingArgs, Mapping[str, Any], Awaitable[Union[Servicev1S3loggingArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">snippets</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1SnippetArgs, Mapping[str, Any], Awaitable[Union[Servicev1SnippetArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1SnippetArgs, Mapping[str, Any], Awaitable[Union[Servicev1SnippetArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">splunks</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1SplunkArgs, Mapping[str, Any], Awaitable[Union[Servicev1SplunkArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1SplunkArgs, Mapping[str, Any], Awaitable[Union[Servicev1SplunkArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">sumologics</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1SumologicArgs, Mapping[str, Any], Awaitable[Union[Servicev1SumologicArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1SumologicArgs, Mapping[str, Any], Awaitable[Union[Servicev1SumologicArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">syslogs</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1SyslogArgs, Mapping[str, Any], Awaitable[Union[Servicev1SyslogArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1SyslogArgs, Mapping[str, Any], Awaitable[Union[Servicev1SyslogArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">vcls</span><span class="p">:</span> <span class="n">Union[List[Union[Servicev1VclArgs, Mapping[str, Any], Awaitable[Union[Servicev1VclArgs, Mapping[str, Any]]], Output[T]]], Awaitable[List[Union[Servicev1VclArgs, Mapping[str, Any], Awaitable[Union[Servicev1VclArgs, Mapping[str, Any]]], Output[T]]]], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">version_comment</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_fastly.servicev1.Servicev1<a class="headerlink" href="#pulumi_fastly.Servicev1.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Servicev1 resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>acls</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1AclArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of ACL configuration blocks.  Defined below.</p></li>
<li><p><strong>activate</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to false. Default true.</p></li>
<li><p><strong>active_version</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The currently active version of your Fastly Service.</p></li>
<li><p><strong>backends</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1BackendArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Backends to service requests from your Domains.
Defined below. Backends must be defined in this argument, or defined in the
<code class="docutils literal notranslate"><span class="pre">vcl</span></code> argument below</p></li>
<li><p><strong>bigqueryloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1BigqueryloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A BigQuery endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>blobstorageloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1BlobstorageloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An Azure Blob Storage endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>cache_settings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1CacheSettingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Cache Settings, allowing you to override</p></li>
<li><p><strong>cloned_version</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The latest cloned version by the provider. The value gets only set after running <code class="docutils literal notranslate"><span class="pre">pulumi</span> <span class="pre">up</span></code>.</p></li>
<li><p><strong>comment</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – An optional comment about the Director.</p></li>
<li><p><strong>conditions</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1ConditionArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of conditions to add logic to any basic
configuration object in this service. Defined below.</p></li>
<li><p><strong>default_host</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Sets the host header.</p></li>
<li><p><strong>default_ttl</strong> (<em>pulumi.Input</em><em>[</em><em>float</em><em>]</em>) – The default Time-to-live (TTL) for
requests.</p></li>
<li><p><strong>dictionaries</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1DictionaryArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of dictionaries that allow the storing of key values pair for use within VCL functions. Defined below.</p></li>
<li><p><strong>directors</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1DirectorArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A director to allow more control over balancing traffic over backends.
when an item is not to be cached based on an above <code class="docutils literal notranslate"><span class="pre">condition</span></code>. Defined below</p></li>
<li><p><strong>domains</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1DomainArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – The domain of the DigitalOcean Spaces endpoint (default “nyc3.digitaloceanspaces.com”).</p></li>
<li><p><strong>dynamicsnippets</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1DynamicsnippetArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of custom, “dynamic” VCL Snippet configuration blocks.  Defined below.</p></li>
<li><p><strong>force_destroy</strong> (<em>pulumi.Input</em><em>[</em><em>bool</em><em>]</em>) – Services that are active cannot be destroyed. In
order to destroy the Service, set <code class="docutils literal notranslate"><span class="pre">force_destroy</span></code> to <code class="docutils literal notranslate"><span class="pre">true</span></code>. Default <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p></li>
<li><p><strong>gcsloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1GcsloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A gcs endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>gzips</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1GzipArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of gzip rules to control automatic gzipping of
content. Defined below.</p></li>
<li><p><strong>headers</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1HeaderArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Headers to manipulate for each request. Defined
below.</p></li>
<li><p><strong>healthchecks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1HealthcheckArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – Name of a defined <code class="docutils literal notranslate"><span class="pre">healthcheck</span></code> to assign to this backend.</p></li>
<li><p><strong>httpsloggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1HttpsloggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An HTTPS endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logentries</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LogentryArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A logentries endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>logging_cloudfiles</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingCloudfileArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Rackspace Cloud Files endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_datadogs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingDatadogArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Datadog endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_digitaloceans</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingDigitaloceanArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A DigitalOcean Spaces endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_elasticsearches</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingElasticsearchArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An Elasticsearch endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_ftps</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingFtpArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An FTP endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_googlepubsubs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingGooglepubsubArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Google Cloud Pub/Sub endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_heroku</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingHerokuArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Heroku endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_honeycombs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingHoneycombArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Honeycomb endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_kafkas</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingKafkaArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Kafka endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_logglies</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingLogglyArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Loggly endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_logshuttles</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingLogshuttleArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Log Shuttle endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_newrelics</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingNewrelicArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A New Relic endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_openstacks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingOpenstackArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An OpenStack endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_scalyrs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingScalyrArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Scalyr endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>logging_sftps</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1LoggingSftpArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – An SFTP endpoint to send streaming logs to.
Defined below.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – A unique name to identify this dictionary.</p></li>
<li><p><strong>papertrails</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1PapertrailArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Papertrail endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>request_settings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1RequestSettingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of Request modifiers. Defined below</p></li>
<li><p><strong>response_objects</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1ResponseObjectArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – Allows you to create synthetic responses that exist entirely on the varnish machine. Useful for creating error or maintenance pages that exists outside the scope of your datacenter. Best when used with Condition objects.</p></li>
<li><p><strong>s3loggings</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1S3loggingArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of S3 Buckets to send streaming logs too.
Defined below.</p></li>
<li><p><strong>snippets</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1SnippetArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A set of custom, “regular” (non-dynamic) VCL Snippet configuration blocks.  Defined below.</p></li>
<li><p><strong>splunks</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1SplunkArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Splunk endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>sumologics</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1SumologicArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A Sumologic endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>syslogs</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1SyslogArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – A syslog endpoint to send streaming logs too.
Defined below.</p></li>
<li><p><strong>vcls</strong> (<em>pulumi.Input</em><em>[</em><em>List</em><em>[</em><em>pulumi.Input</em><em>[</em><em>pulumi.InputType</em><em>[</em><em>'Servicev1VclArgs'</em><em>]</em><em>]</em><em>]</em><em>]</em>) – <p>A set of custom VCL configuration blocks. See the <a class="reference external" href="https://docs.fastly.com/vcl/custom-vcl/uploading-custom-vcl/">Fastly documentation</a> for more information on using custom VCL.</p>
</p></li>
<li><p><strong>version_comment</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – Description field for the version.</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.acls">
<em class="property">property </em><code class="sig-name descname">acls</code><a class="headerlink" href="#pulumi_fastly.Servicev1.acls" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of ACL configuration blocks.  Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.activate">
<em class="property">property </em><code class="sig-name descname">activate</code><a class="headerlink" href="#pulumi_fastly.Servicev1.activate" title="Permalink to this definition">¶</a></dt>
<dd><p>Conditionally prevents the Service from being activated. The apply step will continue to create a new draft version but will not activate it if this is set to false. Default true.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.active_version">
<em class="property">property </em><code class="sig-name descname">active_version</code><a class="headerlink" href="#pulumi_fastly.Servicev1.active_version" title="Permalink to this definition">¶</a></dt>
<dd><p>The currently active version of your Fastly Service.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.backends">
<em class="property">property </em><code class="sig-name descname">backends</code><a class="headerlink" href="#pulumi_fastly.Servicev1.backends" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of Backends to service requests from your Domains.
Defined below. Backends must be defined in this argument, or defined in the
<code class="docutils literal notranslate"><span class="pre">vcl</span></code> argument below</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.bigqueryloggings">
<em class="property">property </em><code class="sig-name descname">bigqueryloggings</code><a class="headerlink" href="#pulumi_fastly.Servicev1.bigqueryloggings" title="Permalink to this definition">¶</a></dt>
<dd><p>A BigQuery endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.blobstorageloggings">
<em class="property">property </em><code class="sig-name descname">blobstorageloggings</code><a class="headerlink" href="#pulumi_fastly.Servicev1.blobstorageloggings" title="Permalink to this definition">¶</a></dt>
<dd><p>An Azure Blob Storage endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.cache_settings">
<em class="property">property </em><code class="sig-name descname">cache_settings</code><a class="headerlink" href="#pulumi_fastly.Servicev1.cache_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of Cache Settings, allowing you to override</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.cloned_version">
<em class="property">property </em><code class="sig-name descname">cloned_version</code><a class="headerlink" href="#pulumi_fastly.Servicev1.cloned_version" title="Permalink to this definition">¶</a></dt>
<dd><p>The latest cloned version by the provider. The value gets only set after running <code class="docutils literal notranslate"><span class="pre">pulumi</span> <span class="pre">up</span></code>.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.comment">
<em class="property">property </em><code class="sig-name descname">comment</code><a class="headerlink" href="#pulumi_fastly.Servicev1.comment" title="Permalink to this definition">¶</a></dt>
<dd><p>An optional comment about the Director.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.conditions">
<em class="property">property </em><code class="sig-name descname">conditions</code><a class="headerlink" href="#pulumi_fastly.Servicev1.conditions" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of conditions to add logic to any basic
configuration object in this service. Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.default_host">
<em class="property">property </em><code class="sig-name descname">default_host</code><a class="headerlink" href="#pulumi_fastly.Servicev1.default_host" title="Permalink to this definition">¶</a></dt>
<dd><p>Sets the host header.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.default_ttl">
<em class="property">property </em><code class="sig-name descname">default_ttl</code><a class="headerlink" href="#pulumi_fastly.Servicev1.default_ttl" title="Permalink to this definition">¶</a></dt>
<dd><p>The default Time-to-live (TTL) for
requests.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.dictionaries">
<em class="property">property </em><code class="sig-name descname">dictionaries</code><a class="headerlink" href="#pulumi_fastly.Servicev1.dictionaries" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of dictionaries that allow the storing of key values pair for use within VCL functions. Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.directors">
<em class="property">property </em><code class="sig-name descname">directors</code><a class="headerlink" href="#pulumi_fastly.Servicev1.directors" title="Permalink to this definition">¶</a></dt>
<dd><p>A director to allow more control over balancing traffic over backends.
when an item is not to be cached based on an above <code class="docutils literal notranslate"><span class="pre">condition</span></code>. Defined below</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.domains">
<em class="property">property </em><code class="sig-name descname">domains</code><a class="headerlink" href="#pulumi_fastly.Servicev1.domains" title="Permalink to this definition">¶</a></dt>
<dd><p>The domain of the DigitalOcean Spaces endpoint (default “nyc3.digitaloceanspaces.com”).</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.dynamicsnippets">
<em class="property">property </em><code class="sig-name descname">dynamicsnippets</code><a class="headerlink" href="#pulumi_fastly.Servicev1.dynamicsnippets" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of custom, “dynamic” VCL Snippet configuration blocks.  Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.force_destroy">
<em class="property">property </em><code class="sig-name descname">force_destroy</code><a class="headerlink" href="#pulumi_fastly.Servicev1.force_destroy" title="Permalink to this definition">¶</a></dt>
<dd><p>Services that are active cannot be destroyed. In
order to destroy the Service, set <code class="docutils literal notranslate"><span class="pre">force_destroy</span></code> to <code class="docutils literal notranslate"><span class="pre">true</span></code>. Default <code class="docutils literal notranslate"><span class="pre">false</span></code>.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.gcsloggings">
<em class="property">property </em><code class="sig-name descname">gcsloggings</code><a class="headerlink" href="#pulumi_fastly.Servicev1.gcsloggings" title="Permalink to this definition">¶</a></dt>
<dd><p>A gcs endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.gzips">
<em class="property">property </em><code class="sig-name descname">gzips</code><a class="headerlink" href="#pulumi_fastly.Servicev1.gzips" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of gzip rules to control automatic gzipping of
content. Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.headers">
<em class="property">property </em><code class="sig-name descname">headers</code><a class="headerlink" href="#pulumi_fastly.Servicev1.headers" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of Headers to manipulate for each request. Defined
below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.healthchecks">
<em class="property">property </em><code class="sig-name descname">healthchecks</code><a class="headerlink" href="#pulumi_fastly.Servicev1.healthchecks" title="Permalink to this definition">¶</a></dt>
<dd><p>Name of a defined <code class="docutils literal notranslate"><span class="pre">healthcheck</span></code> to assign to this backend.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.httpsloggings">
<em class="property">property </em><code class="sig-name descname">httpsloggings</code><a class="headerlink" href="#pulumi_fastly.Servicev1.httpsloggings" title="Permalink to this definition">¶</a></dt>
<dd><p>An HTTPS endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logentries">
<em class="property">property </em><code class="sig-name descname">logentries</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logentries" title="Permalink to this definition">¶</a></dt>
<dd><p>A logentries endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_cloudfiles">
<em class="property">property </em><code class="sig-name descname">logging_cloudfiles</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_cloudfiles" title="Permalink to this definition">¶</a></dt>
<dd><p>A Rackspace Cloud Files endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_datadogs">
<em class="property">property </em><code class="sig-name descname">logging_datadogs</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_datadogs" title="Permalink to this definition">¶</a></dt>
<dd><p>A Datadog endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_digitaloceans">
<em class="property">property </em><code class="sig-name descname">logging_digitaloceans</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_digitaloceans" title="Permalink to this definition">¶</a></dt>
<dd><p>A DigitalOcean Spaces endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_elasticsearches">
<em class="property">property </em><code class="sig-name descname">logging_elasticsearches</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_elasticsearches" title="Permalink to this definition">¶</a></dt>
<dd><p>An Elasticsearch endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_ftps">
<em class="property">property </em><code class="sig-name descname">logging_ftps</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_ftps" title="Permalink to this definition">¶</a></dt>
<dd><p>An FTP endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_googlepubsubs">
<em class="property">property </em><code class="sig-name descname">logging_googlepubsubs</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_googlepubsubs" title="Permalink to this definition">¶</a></dt>
<dd><p>A Google Cloud Pub/Sub endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_heroku">
<em class="property">property </em><code class="sig-name descname">logging_heroku</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_heroku" title="Permalink to this definition">¶</a></dt>
<dd><p>A Heroku endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_honeycombs">
<em class="property">property </em><code class="sig-name descname">logging_honeycombs</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_honeycombs" title="Permalink to this definition">¶</a></dt>
<dd><p>A Honeycomb endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_kafkas">
<em class="property">property </em><code class="sig-name descname">logging_kafkas</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_kafkas" title="Permalink to this definition">¶</a></dt>
<dd><p>A Kafka endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_logglies">
<em class="property">property </em><code class="sig-name descname">logging_logglies</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_logglies" title="Permalink to this definition">¶</a></dt>
<dd><p>A Loggly endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_logshuttles">
<em class="property">property </em><code class="sig-name descname">logging_logshuttles</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_logshuttles" title="Permalink to this definition">¶</a></dt>
<dd><p>A Log Shuttle endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_newrelics">
<em class="property">property </em><code class="sig-name descname">logging_newrelics</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_newrelics" title="Permalink to this definition">¶</a></dt>
<dd><p>A New Relic endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_openstacks">
<em class="property">property </em><code class="sig-name descname">logging_openstacks</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_openstacks" title="Permalink to this definition">¶</a></dt>
<dd><p>An OpenStack endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_scalyrs">
<em class="property">property </em><code class="sig-name descname">logging_scalyrs</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_scalyrs" title="Permalink to this definition">¶</a></dt>
<dd><p>A Scalyr endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.logging_sftps">
<em class="property">property </em><code class="sig-name descname">logging_sftps</code><a class="headerlink" href="#pulumi_fastly.Servicev1.logging_sftps" title="Permalink to this definition">¶</a></dt>
<dd><p>An SFTP endpoint to send streaming logs to.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.name">
<em class="property">property </em><code class="sig-name descname">name</code><a class="headerlink" href="#pulumi_fastly.Servicev1.name" title="Permalink to this definition">¶</a></dt>
<dd><p>A unique name to identify this dictionary.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.papertrails">
<em class="property">property </em><code class="sig-name descname">papertrails</code><a class="headerlink" href="#pulumi_fastly.Servicev1.papertrails" title="Permalink to this definition">¶</a></dt>
<dd><p>A Papertrail endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.request_settings">
<em class="property">property </em><code class="sig-name descname">request_settings</code><a class="headerlink" href="#pulumi_fastly.Servicev1.request_settings" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of Request modifiers. Defined below</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.response_objects">
<em class="property">property </em><code class="sig-name descname">response_objects</code><a class="headerlink" href="#pulumi_fastly.Servicev1.response_objects" title="Permalink to this definition">¶</a></dt>
<dd><p>Allows you to create synthetic responses that exist entirely on the varnish machine. Useful for creating error or maintenance pages that exists outside the scope of your datacenter. Best when used with Condition objects.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.s3loggings">
<em class="property">property </em><code class="sig-name descname">s3loggings</code><a class="headerlink" href="#pulumi_fastly.Servicev1.s3loggings" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of S3 Buckets to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.snippets">
<em class="property">property </em><code class="sig-name descname">snippets</code><a class="headerlink" href="#pulumi_fastly.Servicev1.snippets" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of custom, “regular” (non-dynamic) VCL Snippet configuration blocks.  Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.splunks">
<em class="property">property </em><code class="sig-name descname">splunks</code><a class="headerlink" href="#pulumi_fastly.Servicev1.splunks" title="Permalink to this definition">¶</a></dt>
<dd><p>A Splunk endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.sumologics">
<em class="property">property </em><code class="sig-name descname">sumologics</code><a class="headerlink" href="#pulumi_fastly.Servicev1.sumologics" title="Permalink to this definition">¶</a></dt>
<dd><p>A Sumologic endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.syslogs">
<em class="property">property </em><code class="sig-name descname">syslogs</code><a class="headerlink" href="#pulumi_fastly.Servicev1.syslogs" title="Permalink to this definition">¶</a></dt>
<dd><p>A syslog endpoint to send streaming logs too.
Defined below.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.vcls">
<em class="property">property </em><code class="sig-name descname">vcls</code><a class="headerlink" href="#pulumi_fastly.Servicev1.vcls" title="Permalink to this definition">¶</a></dt>
<dd><p>A set of custom VCL configuration blocks. See the <a class="reference external" href="https://docs.fastly.com/vcl/custom-vcl/uploading-custom-vcl/">Fastly documentation</a> for more information on using custom VCL.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.version_comment">
<em class="property">property </em><code class="sig-name descname">version_comment</code><a class="headerlink" href="#pulumi_fastly.Servicev1.version_comment" title="Permalink to this definition">¶</a></dt>
<dd><p>Description field for the version.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Servicev1.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Servicev1.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Servicev1.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py class">
<dt id="pulumi_fastly.Userv1">
<em class="property">class </em><code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">Userv1</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">login</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">name</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">role</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__props__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__name__</span><span class="o">=</span><span class="default_value">None</span></em>, <em class="sig-param"><span class="n">__opts__</span><span class="o">=</span><span class="default_value">None</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Userv1" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides a Fastly User, representing the configuration for a user account for interacting with Fastly.</p>
<p>The User resource requires a login and name, and optionally a role.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">demo</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">Userv1</span><span class="p">(</span><span class="s2">&quot;demo&quot;</span><span class="p">,</span> <span class="n">login</span><span class="o">=</span><span class="s2">&quot;demo@example.com&quot;</span><span class="p">)</span>
</pre></div>
</div>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The name of the resource.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>login</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The email address, which is the login name, of the User.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The real life name of the user.</p></li>
<li><p><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The role of this user. Can be <code class="docutils literal notranslate"><span class="pre">user</span></code> (the default), <code class="docutils literal notranslate"><span class="pre">billing</span></code>, <code class="docutils literal notranslate"><span class="pre">engineer</span></code>, or <code class="docutils literal notranslate"><span class="pre">superuser</span></code>. For detailed information on the abilities granted to each role, see <a class="reference external" href="https://docs.fastly.com/en/guides/configuring-user-roles-and-permissions#user-roles-and-what-they-can-do">Fastly’s Documentation on User roles</a>.</p></li>
</ul>
</dd>
</dl>
<dl class="py method">
<dt id="pulumi_fastly.Userv1.get">
<em class="property">static </em><code class="sig-name descname">get</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">resource_name</span><span class="p">:</span> <span class="n">str</span></em>, <em class="sig-param"><span class="n">id</span><span class="p">:</span> <span class="n">Union<span class="p">[</span>str<span class="p">, </span>Awaitable<span class="p">[</span>str<span class="p">]</span><span class="p">, </span>Output<span class="p">[</span>T<span class="p">]</span><span class="p">]</span></span></em>, <em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.resource.ResourceOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">login</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">name</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em>, <em class="sig-param"><span class="n">role</span><span class="p">:</span> <span class="n">Union[str, Awaitable[str], Output[T], None]</span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_fastly.userv1.Userv1<a class="headerlink" href="#pulumi_fastly.Userv1.get" title="Permalink to this definition">¶</a></dt>
<dd><p>Get an existing Userv1 resource’s state with the given name, id, and optional extra
properties used to qualify the lookup.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><ul class="simple">
<li><p><strong>resource_name</strong> (<em>str</em>) – The unique name of the resulting resource.</p></li>
<li><p><strong>id</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The unique provider ID of the resource to lookup.</p></li>
<li><p><strong>opts</strong> (<a class="reference internal" href="../pulumi/#pulumi.ResourceOptions" title="pulumi.ResourceOptions"><em>pulumi.ResourceOptions</em></a>) – Options for the resource.</p></li>
<li><p><strong>login</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The email address, which is the login name, of the User.</p></li>
<li><p><strong>name</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – The real life name of the user.</p></li>
<li><p><strong>role</strong> (<em>pulumi.Input</em><em>[</em><em>str</em><em>]</em>) – <p>The role of this user. Can be <code class="docutils literal notranslate"><span class="pre">user</span></code> (the default), <code class="docutils literal notranslate"><span class="pre">billing</span></code>, <code class="docutils literal notranslate"><span class="pre">engineer</span></code>, or <code class="docutils literal notranslate"><span class="pre">superuser</span></code>. For detailed information on the abilities granted to each role, see <a class="reference external" href="https://docs.fastly.com/en/guides/configuring-user-roles-and-permissions#user-roles-and-what-they-can-do">Fastly’s Documentation on User roles</a>.</p>
</p></li>
</ul>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Userv1.login">
<em class="property">property </em><code class="sig-name descname">login</code><a class="headerlink" href="#pulumi_fastly.Userv1.login" title="Permalink to this definition">¶</a></dt>
<dd><p>The email address, which is the login name, of the User.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Userv1.name">
<em class="property">property </em><code class="sig-name descname">name</code><a class="headerlink" href="#pulumi_fastly.Userv1.name" title="Permalink to this definition">¶</a></dt>
<dd><p>The real life name of the user.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Userv1.role">
<em class="property">property </em><code class="sig-name descname">role</code><a class="headerlink" href="#pulumi_fastly.Userv1.role" title="Permalink to this definition">¶</a></dt>
<dd><p>The role of this user. Can be <code class="docutils literal notranslate"><span class="pre">user</span></code> (the default), <code class="docutils literal notranslate"><span class="pre">billing</span></code>, <code class="docutils literal notranslate"><span class="pre">engineer</span></code>, or <code class="docutils literal notranslate"><span class="pre">superuser</span></code>. For detailed information on the abilities granted to each role, see <a class="reference external" href="https://docs.fastly.com/en/guides/configuring-user-roles-and-permissions#user-roles-and-what-they-can-do">Fastly’s Documentation on User roles</a>.</p>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Userv1.translate_output_property">
<code class="sig-name descname">translate_output_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Userv1.translate_output_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of output properties
into a format of their choosing before writing those properties to the resource object.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

<dl class="py method">
<dt id="pulumi_fastly.Userv1.translate_input_property">
<code class="sig-name descname">translate_input_property</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">prop</span></em><span class="sig-paren">)</span><a class="headerlink" href="#pulumi_fastly.Userv1.translate_input_property" title="Permalink to this definition">¶</a></dt>
<dd><p>Provides subclasses of Resource an opportunity to translate names of input properties into
a format of their choosing before sending those properties to the Pulumi engine.</p>
<dl class="field-list simple">
<dt class="field-odd">Parameters</dt>
<dd class="field-odd"><p><strong>prop</strong> (<em>str</em>) – A property name.</p>
</dd>
<dt class="field-even">Returns</dt>
<dd class="field-even"><p>A potentially transformed property name.</p>
</dd>
<dt class="field-odd">Return type</dt>
<dd class="field-odd"><p>str</p>
</dd>
</dl>
</dd></dl>

</dd></dl>

<dl class="py function">
<dt id="pulumi_fastly.get_fastly_ip_ranges">
<code class="sig-prename descclassname">pulumi_fastly.</code><code class="sig-name descname">get_fastly_ip_ranges</code><span class="sig-paren">(</span><em class="sig-param"><span class="n">opts</span><span class="p">:</span> <span class="n">Optional<span class="p">[</span>pulumi.invoke.InvokeOptions<span class="p">]</span></span> <span class="o">=</span> <span class="default_value">None</span></em><span class="sig-paren">)</span> &#x2192; pulumi_fastly.get_fastly_ip_ranges.AwaitableGetFastlyIpRangesResult<a class="headerlink" href="#pulumi_fastly.get_fastly_ip_ranges" title="Permalink to this definition">¶</a></dt>
<dd><p>Use this data source to get the <a class="reference external" href="https://docs.fastly.com/guides/securing-communications/accessing-fastlys-ip-ranges">IP ranges</a> of Fastly edge nodes.</p>
<div class="highlight-python notranslate"><div class="highlight"><pre><span></span><span class="kn">import</span> <span class="nn">pulumi</span>
<span class="kn">import</span> <span class="nn">pulumi_aws</span> <span class="k">as</span> <span class="nn">aws</span>
<span class="kn">import</span> <span class="nn">pulumi_fastly</span> <span class="k">as</span> <span class="nn">fastly</span>

<span class="n">fastly</span> <span class="o">=</span> <span class="n">fastly</span><span class="o">.</span><span class="n">get_fastly_ip_ranges</span><span class="p">()</span>
<span class="n">from_fastly</span> <span class="o">=</span> <span class="n">aws</span><span class="o">.</span><span class="n">ec2</span><span class="o">.</span><span class="n">SecurityGroup</span><span class="p">(</span><span class="s2">&quot;fromFastly&quot;</span><span class="p">,</span> <span class="n">ingress</span><span class="o">=</span><span class="p">[{</span>
    <span class="s2">&quot;cidr_blocks&quot;</span><span class="p">:</span> <span class="n">fastly</span><span class="o">.</span><span class="n">cidr_blocks</span><span class="p">,</span>
    <span class="s2">&quot;from_port&quot;</span><span class="p">:</span> <span class="s2">&quot;443&quot;</span><span class="p">,</span>
    <span class="s2">&quot;ipv6_cidr_blocks&quot;</span><span class="p">:</span> <span class="n">fastly</span><span class="o">.</span><span class="n">ipv6_cidr_blocks</span><span class="p">,</span>
    <span class="s2">&quot;protocol&quot;</span><span class="p">:</span> <span class="s2">&quot;tcp&quot;</span><span class="p">,</span>
    <span class="s2">&quot;to_port&quot;</span><span class="p">:</span> <span class="s2">&quot;443&quot;</span><span class="p">,</span>
<span class="p">}])</span>
</pre></div>
</div>
</dd></dl>

</div>
