---
title: StreamProviderOptions.DefaultPath
second_title: Aspose.Cells for .NET API Reference
description: StreamProviderOptions property. The default pathURL saved in generated html file for the referred source. For example the sheet data saved in xxx_files/sheet001.htm the url used in the main html file should be like srcxxx_files/sheet001.htm
type: docs
url: /net/aspose.cells/streamprovideroptions/defaultpath/
---
## StreamProviderOptions.DefaultPath property

The default path(URL) saved in generated html file for the referred source. For example, the sheet data saved in xxx_files/sheet001.htm, the url used in the main html file should be like "src="xxx_files/sheet001.htm""

```csharp
public string DefaultPath { get; }
```

### Examples

```csharp
// Called: Console.WriteLine(&amp;quot;Using ms1 for &amp;quot; + opts.DefaultPath);
public void Property_DefaultPath(StreamProviderOptions opts)
            {
                if (opts.DefaultPath.IndexOf(&quot;1.&quot;) &gt; 0)
                {
                    Console.WriteLine(&quot;Using ms1 for &quot; + opts.DefaultPath);
                    opts.Stream = _ms1;
                    _initCount++;
                }
                else if (opts.DefaultPath.IndexOf(&quot;2.&quot;) &gt; 0)
                {
                    Console.WriteLine(&quot;Using ms2 for &quot; + opts.DefaultPath);
                    opts.Stream = _ms2;
                    _initCount++;
                }
                else
                {
                    Console.WriteLine(&quot;Path for others: &quot; + opts.DefaultPath);
                    opts.Stream = new MemoryStream();
                }
            }
```

### See Also

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


