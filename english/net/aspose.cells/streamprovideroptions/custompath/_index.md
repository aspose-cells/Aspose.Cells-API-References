---
title: StreamProviderOptions.CustomPath
second_title: Aspose.Cells for .NET API Reference
description: StreamProviderOptions property. The user custom pathURL saved in generated html file for the referred source. If not defined by user DefaultPath will be used. For example the sheet data will be saved by user to d/sheet001.htm the url used in the main html file should be d/sheet001.htm or other valid relative path that can be accessed by the main html file
type: docs
url: /net/aspose.cells/streamprovideroptions/custompath/
---
## StreamProviderOptions.CustomPath property

The user custom path(URL) saved in generated html file for the referred source. If not defined by user, DefaultPath will be used. For example, the sheet data will be saved by user to d:/sheet001.htm, the url used in the main html file should be "d:/sheet001.htm" or other valid relative path that can be accessed by the main html file.

```csharp
public string CustomPath { get; set; }
```

### Examples

```csharp
// Called: options.CustomPath = &amp;quot;image.png&amp;quot;;
void IStreamProvider.Property_CustomPath(StreamProviderOptions options)
            {
                streamProviderOptions = options;
                string resourcePath = Path.Combine(_outputDirectory, &quot;image.png&quot;);
                options.Stream = new FileStream(resourcePath, FileMode.Create);
                options.CustomPath = &quot;image.png&quot;;
            }
```

### See Also

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


