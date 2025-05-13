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
// Called: options.Stream = new MemoryStream();
public void StreamProviderOptions_Property_Stream(StreamProviderOptions options)
            {
                if (options.DefaultPath == null)
                {
                    options.Stream = new MemoryStream();
                }
                else
                {
                    string path = outputDir + Path.GetFileName(options.DefaultPath);
                    options.CustomPath = path;
                    Directory.CreateDirectory(Path.GetDirectoryName(path));
                    options.Stream = File.Create(path);
                }
            }
```

### See Also

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


