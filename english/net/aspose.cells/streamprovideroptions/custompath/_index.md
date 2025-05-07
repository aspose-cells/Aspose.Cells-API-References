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
// Called: options.CustomPath = resourceName;
void IStreamProvider.Property_CustomPath(StreamProviderOptions options)
            {
                string resourceName = Path.GetFileName(options.DefaultPath);

                string resourcePath = Path.Combine(CreateFolder(Constants.HtmlDestPath+ "NET46383"), resourceName);

                FileStream resourceStream = new FileStream(resourcePath, FileMode.Create);
                options.Stream = resourceStream;

                options.CustomPath = resourceName;
            }
```

### See Also

* class [StreamProviderOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


