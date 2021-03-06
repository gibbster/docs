
---
title: "GetZoneRecords"
title_tag: "Function GetZoneRecords | Module pvtz | Package AliCloud"
meta_desc: "Explore the GetZoneRecords function of the pvtz module, including examples, input properties, output properties, and supporting types. This data source provides Private Zone Records resource information owned by an Alibaba Cloud account."
---



<!-- WARNING: this file was generated by Pulumi Docs Generator. -->
<!-- Do not edit by hand unless you're certain you know what you are doing! -->

This data source provides Private Zone Records resource information owned by an Alibaba Cloud account.

{{% examples %}}
## Example Usage

{{< chooser language "typescript,python,go,csharp" / >}}

{{% example csharp %}}
```csharp
using Pulumi;
using AliCloud = Pulumi.AliCloud;

class MyStack : Stack
{
    public MyStack()
    {
        var recordsDs = Output.Create(AliCloud.Pvtz.GetZoneRecords.InvokeAsync(new AliCloud.Pvtz.GetZoneRecordsArgs
        {
            Keyword = alicloud_pvtz_zone_record.Foo.Value,
            ZoneId = alicloud_pvtz_zone.Basic.Id,
        }));
        this.FirstRecordId = recordsDs.Apply(recordsDs => recordsDs.Records[0].Id);
    }

    [Output("firstRecordId")]
    public Output<string> FirstRecordId { get; set; }
}
```

{{% /example %}}

{{% example go %}}
```go
package main

import (
	"github.com/pulumi/pulumi-alicloud/sdk/v2/go/alicloud/pvtz"
	"github.com/pulumi/pulumi/sdk/v2/go/pulumi"
)

func main() {
	pulumi.Run(func(ctx *pulumi.Context) error {
		opt0 := alicloud_pvtz_zone_record.Foo.Value
		recordsDs, err := pvtz.GetZoneRecords(ctx, &pvtz.GetZoneRecordsArgs{
			Keyword: &opt0,
			ZoneId:  alicloud_pvtz_zone.Basic.Id,
		}, nil)
		if err != nil {
			return err
		}
		ctx.Export("firstRecordId", recordsDs.Records[0].Id)
		return nil
	})
}
```

{{% /example %}}

{{% example python %}}
```python
import pulumi
import pulumi_alicloud as alicloud

records_ds = alicloud.pvtz.get_zone_records(keyword=alicloud_pvtz_zone_record["foo"]["value"],
    zone_id=alicloud_pvtz_zone["basic"]["id"])
pulumi.export("firstRecordId", records_ds.records[0].id)
```

{{% /example %}}

{{% example typescript %}}

```typescript
import * as pulumi from "@pulumi/pulumi";
import * as alicloud from "@pulumi/alicloud";

const recordsDs = pulumi.all([alicloud_pvtz_zone_record_foo.value, alicloud_pvtz_zone_basic.id]).apply(([value, id]) => alicloud.pvtz.getZoneRecords({
    keyword: value,
    zoneId: id,
}, { async: true }));

export const firstRecordId = recordsDs.records[0].id;
```

{{% /example %}}

{{% /examples %}}


## Using GetZoneRecords {#using}

{{< chooser language "typescript,python,go,csharp" / >}}


{{% choosable language nodejs %}}
<div class="highlight"><pre class="chroma"><code class="language-typescript" data-lang="typescript"><span class="k">function </span>getZoneRecords<span class="p">(</span><span class="nx">args</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/alicloud/pvtz/#GetZoneRecordsArgs">GetZoneRecordsArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p">?:</span> <span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/pulumi/#InvokeOptions">InvokeOptions</a></span><span class="p">): Promise&lt;<span class="nx"><a href="/docs/reference/pkg/nodejs/pulumi/alicloud/pvtz/#GetZoneRecordsResult">GetZoneRecordsResult</a></span>></span></code></pre></div>
{{% /choosable %}}


{{% choosable language python %}}
<div class="highlight"><pre class="chroma"><code class="language-python" data-lang="python"><span class="k">def </span>get_zone_records(</span><span class="nx">ids</span><span class="p">:</span> <span class="nx">Optional[Sequence[str]]</span> = None<span class="p">, </span><span class="nx">keyword</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">output_file</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">zone_id</span><span class="p">:</span> <span class="nx">Optional[str]</span> = None<span class="p">, </span><span class="nx">opts</span><span class="p">:</span> <span class="nx"><a href="/docs/reference/pkg/python/pulumi/#pulumi.InvokeOptions">Optional[InvokeOptions]</a></span> = None<span class="p">) -&gt;</span> GetZoneRecordsResult</code></pre></div>
{{% /choosable %}}


{{% choosable language go %}}
<div class="highlight"><pre class="chroma"><code class="language-go" data-lang="go"><span class="k">func </span>GetZoneRecords<span class="p">(</span><span class="nx">ctx</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#Context">Context</a></span><span class="p">, </span><span class="nx">args</span><span class="p"> *</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/v2/go/alicloud/pvtz?tab=doc#GetZoneRecordsArgs">GetZoneRecordsArgs</a></span><span class="p">, </span><span class="nx">opts</span><span class="p"> ...</span><span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi/sdk/v2/go/pulumi?tab=doc#InvokeOption">InvokeOption</a></span><span class="p">) (*<span class="nx"><a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/v2/go/alicloud/pvtz?tab=doc#GetZoneRecordsResult">GetZoneRecordsResult</a></span>, error)</span></code></pre></div>

{{% /choosable %}}


{{% choosable language csharp %}}
<div class="highlight"><pre class="chroma"><code class="language-csharp" data-lang="csharp"><span class="k">public static class </span><span class="nx">GetZoneRecords </span><span class="p">{</span><span class="k">
    public static </span>Task&lt;<span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.AliCloud/Pulumi.AliCloud.Pvtz.GetZoneRecordsResult.html">GetZoneRecordsResult</a></span>> <span class="p">InvokeAsync(</span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi.AliCloud/Pulumi.AliCloud.Pvtz.GetZoneRecordsArgs.html">GetZoneRecordsArgs</a></span><span class="p"> </span><span class="nx">args<span class="p">, </span><span class="nx"><a href="/docs/reference/pkg/dotnet/Pulumi/Pulumi.InvokeOptions.html">InvokeOptions</a></span><span class="p">? </span><span class="nx">opts = null<span class="p">)</span><span class="p">
}</span></code></pre></div>
{{% /choosable %}}



The following arguments are supported:



{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="zoneid_csharp">
<a href="#zoneid_csharp" style="color: inherit; text-decoration: inherit;">Zone<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}ID of the Private Zone.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="ids_csharp">
<a href="#ids_csharp" style="color: inherit; text-decoration: inherit;">Ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">List&lt;string&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of Private Zone Record IDs.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="keyword_csharp">
<a href="#keyword_csharp" style="color: inherit; text-decoration: inherit;">Keyword</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}Keyword for record rr and value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="outputfile_csharp">
<a href="#outputfile_csharp" style="color: inherit; text-decoration: inherit;">Output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="zoneid_go">
<a href="#zoneid_go" style="color: inherit; text-decoration: inherit;">Zone<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}ID of the Private Zone.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="ids_go">
<a href="#ids_go" style="color: inherit; text-decoration: inherit;">Ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">[]string</a></span>
    </dt>
    <dd>{{% md %}}A list of Private Zone Record IDs.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="keyword_go">
<a href="#keyword_go" style="color: inherit; text-decoration: inherit;">Keyword</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}Keyword for record rr and value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="outputfile_go">
<a href="#outputfile_go" style="color: inherit; text-decoration: inherit;">Output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="zoneid_nodejs">
<a href="#zoneid_nodejs" style="color: inherit; text-decoration: inherit;">zone<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}ID of the Private Zone.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="ids_nodejs">
<a href="#ids_nodejs" style="color: inherit; text-decoration: inherit;">ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string[]</a></span>
    </dt>
    <dd>{{% md %}}A list of Private Zone Record IDs.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="keyword_nodejs">
<a href="#keyword_nodejs" style="color: inherit; text-decoration: inherit;">keyword</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}Keyword for record rr and value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="outputfile_nodejs">
<a href="#outputfile_nodejs" style="color: inherit; text-decoration: inherit;">output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="zone_id_python">
<a href="#zone_id_python" style="color: inherit; text-decoration: inherit;">zone_<wbr>id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}ID of the Private Zone.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="ids_python">
<a href="#ids_python" style="color: inherit; text-decoration: inherit;">ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">Sequence[str]</a></span>
    </dt>
    <dd>{{% md %}}A list of Private Zone Record IDs.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="keyword_python">
<a href="#keyword_python" style="color: inherit; text-decoration: inherit;">keyword</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}Keyword for record rr and value.
{{% /md %}}</dd>

    <dt class="property-optional"
            title="Optional">
        <span id="output_file_python">
<a href="#output_file_python" style="color: inherit; text-decoration: inherit;">output_<wbr>file</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## GetZoneRecords Result {#result}

The following output properties are available:




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="ids_csharp">
<a href="#ids_csharp" style="color: inherit; text-decoration: inherit;">Ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">List&lt;string&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of Private Zone Record IDs.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="records_csharp">
<a href="#records_csharp" style="color: inherit; text-decoration: inherit;">Records</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getzonerecordsrecord">List&lt;Pulumi.<wbr>Ali<wbr>Cloud.<wbr>Pvtz.<wbr>Outputs.<wbr>Get<wbr>Zone<wbr>Records<wbr>Record&gt;</a></span>
    </dt>
    <dd>{{% md %}}A list of zone records. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="zoneid_csharp">
<a href="#zoneid_csharp" style="color: inherit; text-decoration: inherit;">Zone<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="keyword_csharp">
<a href="#keyword_csharp" style="color: inherit; text-decoration: inherit;">Keyword</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="outputfile_csharp">
<a href="#outputfile_csharp" style="color: inherit; text-decoration: inherit;">Output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="ids_go">
<a href="#ids_go" style="color: inherit; text-decoration: inherit;">Ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">[]string</a></span>
    </dt>
    <dd>{{% md %}}A list of Private Zone Record IDs.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="records_go">
<a href="#records_go" style="color: inherit; text-decoration: inherit;">Records</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getzonerecordsrecord">[]Get<wbr>Zone<wbr>Records<wbr>Record</a></span>
    </dt>
    <dd>{{% md %}}A list of zone records. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="zoneid_go">
<a href="#zoneid_go" style="color: inherit; text-decoration: inherit;">Zone<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="keyword_go">
<a href="#keyword_go" style="color: inherit; text-decoration: inherit;">Keyword</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="outputfile_go">
<a href="#outputfile_go" style="color: inherit; text-decoration: inherit;">Output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="ids_nodejs">
<a href="#ids_nodejs" style="color: inherit; text-decoration: inherit;">ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string[]</a></span>
    </dt>
    <dd>{{% md %}}A list of Private Zone Record IDs.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="records_nodejs">
<a href="#records_nodejs" style="color: inherit; text-decoration: inherit;">records</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getzonerecordsrecord">Get<wbr>Zone<wbr>Records<wbr>Record[]</a></span>
    </dt>
    <dd>{{% md %}}A list of zone records. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="zoneid_nodejs">
<a href="#zoneid_nodejs" style="color: inherit; text-decoration: inherit;">zone<wbr>Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="keyword_nodejs">
<a href="#keyword_nodejs" style="color: inherit; text-decoration: inherit;">keyword</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="outputfile_nodejs">
<a href="#outputfile_nodejs" style="color: inherit; text-decoration: inherit;">output<wbr>File</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-"
            title="">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}The provider-assigned unique ID for this managed resource.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="ids_python">
<a href="#ids_python" style="color: inherit; text-decoration: inherit;">ids</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">Sequence[str]</a></span>
    </dt>
    <dd>{{% md %}}A list of Private Zone Record IDs.
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="records_python">
<a href="#records_python" style="color: inherit; text-decoration: inherit;">records</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="#getzonerecordsrecord">Sequence[Get<wbr>Zone<wbr>Records<wbr>Record]</a></span>
    </dt>
    <dd>{{% md %}}A list of zone records. Each element contains the following attributes:
{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="zone_id_python">
<a href="#zone_id_python" style="color: inherit; text-decoration: inherit;">zone_<wbr>id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="keyword_python">
<a href="#keyword_python" style="color: inherit; text-decoration: inherit;">keyword</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-"
            title="">
        <span id="output_file_python">
<a href="#output_file_python" style="color: inherit; text-decoration: inherit;">output_<wbr>file</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

</dl>
{{% /choosable %}}








## Supporting Types


<h4 id="getzonerecordsrecord">Get<wbr>Zone<wbr>Records<wbr>Record</h4>
{{% choosable language nodejs %}}
> See the   <a href="/docs/reference/pkg/nodejs/pulumi/alicloud/types/output/#GetZoneRecordsRecord">output</a> API doc for this type.
{{% /choosable %}}

{{% choosable language go %}}
> See the   <a href="https://pkg.go.dev/github.com/pulumi/pulumi-alicloud/sdk/v2/go/alicloud/pvtz?tab=doc#GetZoneRecordsRecord">output</a> API doc for this type.
{{% /choosable %}}
{{% choosable language csharp %}}
> See the   <a href="/docs/reference/pkg/dotnet/Pulumi.AliCloud/Pulumi.AliCloud.Pvtz.Outputs.GetZoneRecordsRecord.html">output</a> API doc for this type.
{{% /choosable %}}




{{% choosable language csharp %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="id_csharp">
<a href="#id_csharp" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">int</a></span>
    </dt>
    <dd>{{% md %}}ID of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="priority_csharp">
<a href="#priority_csharp" style="color: inherit; text-decoration: inherit;">Priority</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">int</a></span>
    </dt>
    <dd>{{% md %}}Priority of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="resourcerecord_csharp">
<a href="#resourcerecord_csharp" style="color: inherit; text-decoration: inherit;">Resource<wbr>Record</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}Resource record of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="status_csharp">
<a href="#status_csharp" style="color: inherit; text-decoration: inherit;">Status</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="ttl_csharp">
<a href="#ttl_csharp" style="color: inherit; text-decoration: inherit;">Ttl</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">int</a></span>
    </dt>
    <dd>{{% md %}}Ttl of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="type_csharp">
<a href="#type_csharp" style="color: inherit; text-decoration: inherit;">Type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}Type of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="value_csharp">
<a href="#value_csharp" style="color: inherit; text-decoration: inherit;">Value</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/builtin-types/built-in-types">string</a></span>
    </dt>
    <dd>{{% md %}}Value of the Private Zone Record.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language go %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="id_go">
<a href="#id_go" style="color: inherit; text-decoration: inherit;">Id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#integer">int</a></span>
    </dt>
    <dd>{{% md %}}ID of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="priority_go">
<a href="#priority_go" style="color: inherit; text-decoration: inherit;">Priority</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#integer">int</a></span>
    </dt>
    <dd>{{% md %}}Priority of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="resourcerecord_go">
<a href="#resourcerecord_go" style="color: inherit; text-decoration: inherit;">Resource<wbr>Record</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}Resource record of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="status_go">
<a href="#status_go" style="color: inherit; text-decoration: inherit;">Status</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="ttl_go">
<a href="#ttl_go" style="color: inherit; text-decoration: inherit;">Ttl</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#integer">int</a></span>
    </dt>
    <dd>{{% md %}}Ttl of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="type_go">
<a href="#type_go" style="color: inherit; text-decoration: inherit;">Type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}Type of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="value_go">
<a href="#value_go" style="color: inherit; text-decoration: inherit;">Value</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://golang.org/pkg/builtin/#string">string</a></span>
    </dt>
    <dd>{{% md %}}Value of the Private Zone Record.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language nodejs %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="id_nodejs">
<a href="#id_nodejs" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/integer">number</a></span>
    </dt>
    <dd>{{% md %}}ID of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="priority_nodejs">
<a href="#priority_nodejs" style="color: inherit; text-decoration: inherit;">priority</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/integer">number</a></span>
    </dt>
    <dd>{{% md %}}Priority of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="resourcerecord_nodejs">
<a href="#resourcerecord_nodejs" style="color: inherit; text-decoration: inherit;">resource<wbr>Record</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}Resource record of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="status_nodejs">
<a href="#status_nodejs" style="color: inherit; text-decoration: inherit;">status</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="ttl_nodejs">
<a href="#ttl_nodejs" style="color: inherit; text-decoration: inherit;">ttl</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/integer">number</a></span>
    </dt>
    <dd>{{% md %}}Ttl of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="type_nodejs">
<a href="#type_nodejs" style="color: inherit; text-decoration: inherit;">type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}Type of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="value_nodejs">
<a href="#value_nodejs" style="color: inherit; text-decoration: inherit;">value</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/string">string</a></span>
    </dt>
    <dd>{{% md %}}Value of the Private Zone Record.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}


{{% choosable language python %}}
<dl class="resources-properties">

    <dt class="property-required"
            title="Required">
        <span id="id_python">
<a href="#id_python" style="color: inherit; text-decoration: inherit;">id</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">int</a></span>
    </dt>
    <dd>{{% md %}}ID of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="priority_python">
<a href="#priority_python" style="color: inherit; text-decoration: inherit;">priority</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">int</a></span>
    </dt>
    <dd>{{% md %}}Priority of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="resource_record_python">
<a href="#resource_record_python" style="color: inherit; text-decoration: inherit;">resource_<wbr>record</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}Resource record of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="status_python">
<a href="#status_python" style="color: inherit; text-decoration: inherit;">status</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="ttl_python">
<a href="#ttl_python" style="color: inherit; text-decoration: inherit;">ttl</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">int</a></span>
    </dt>
    <dd>{{% md %}}Ttl of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="type_python">
<a href="#type_python" style="color: inherit; text-decoration: inherit;">type</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}Type of the Private Zone Record.
{{% /md %}}</dd>

    <dt class="property-required"
            title="Required">
        <span id="value_python">
<a href="#value_python" style="color: inherit; text-decoration: inherit;">value</a>
</span> 
        <span class="property-indicator"></span>
        <span class="property-type"><a href="https://docs.python.org/3/library/stdtypes.html">str</a></span>
    </dt>
    <dd>{{% md %}}Value of the Private Zone Record.
{{% /md %}}</dd>

</dl>
{{% /choosable %}}









<h2 id="package-details">Package Details</h2>
<dl class="package-details">
	<dt>Repository</dt>
	<dd><a href="https://github.com/pulumi/pulumi-alicloud">https://github.com/pulumi/pulumi-alicloud</a></dd>
	<dt>License</dt>
	<dd>Apache-2.0</dd>
	<dt>Notes</dt>
	<dd>This Pulumi package is based on the [`alicloud` Terraform Provider](https://github.com/aliyun/terraform-provider-alicloud).</dd>
</dl>

