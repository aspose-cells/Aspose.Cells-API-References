---
title: StreamProviderOptions.Stream
second_title: Aspose.Cells for .NET API Reference
description: StreamProviderOptions property. Gets/Sets the stream
type: docs
url: /net/aspose.cells/streamprovideroptions/stream/
---
## StreamProviderOptions.Stream property

Gets/Sets the stream

```csharp
public Stream Stream { get; set; }
```

### Examples

```csharp
// Called: opts.Stream = _ms1;
public void Property_Stream(StreamProviderOptions opts)
            {
                if (opts.DefaultPath.IndexOf("1.") > 0)
                {
                    Console.WriteLine("Using ms1 for " + opts.DefaultPath);
                    opts.Stream = _ms1;
                    _initCount++;
                }
                else if (opts.DefaultPath.IndexOf("2.") > 0)
                {
                    Console.WriteLine("Using ms2 for " + opts.DefaultPath);
                    opts.Stream = _ms2;
                    _initCount++;
                }
                else
                {
                    Console.WriteLine("Path for others: " + opts.DefaultPath);
                    opts.Stream = new MemoryStream();
                }
            }
```

### See Also

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


