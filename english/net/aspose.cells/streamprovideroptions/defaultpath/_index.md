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
// Called: Assert.Fail("Stream should be ms1, but now it is not: for " + opts.DefaultPath);
public void StreamProviderOptions_Property_DefaultPath(StreamProviderOptions opts)
            {
                if (opts.DefaultPath.IndexOf("1.") > 0)
                {
                    Console.WriteLine("Closing stream for " + opts.DefaultPath);
                    if (opts.Stream != _ms1)
                    {
                        Assert.Fail("Stream should be ms1, but now it is not: for " + opts.DefaultPath);
                    }
                    _closeCount++;
                }
                else if (opts.DefaultPath.IndexOf("2.") > 0)
                {
                    Console.WriteLine("Closing stream for " + opts.DefaultPath);
                    if (opts.Stream != _ms2)
                    {
                        Assert.Fail("Stream should be ms1, but now it is not: for " + opts.DefaultPath);
                    }
                    _closeCount++;
                }
                else
                {
                    Console.WriteLine("Path for others: " + opts.DefaultPath);
                }
            }
```

### See Also

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


