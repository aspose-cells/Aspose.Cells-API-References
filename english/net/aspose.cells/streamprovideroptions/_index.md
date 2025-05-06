---
title: Class StreamProviderOptions
second_title: Aspose.Cells for .NET API Reference
description: Aspose.Cells.StreamProviderOptions class. Represents the stream options
type: docs
url: /net/aspose.cells/streamprovideroptions/
---
## StreamProviderOptions class

Represents the stream options.

```csharp
public class StreamProviderOptions
```

## Constructors

| Name | Description |
| --- | --- |
| [StreamProviderOptions](streamprovideroptions/#constructor)() | Initializes a new instance of the `StreamProviderOptions` class. |
| [StreamProviderOptions](streamprovideroptions/#constructor_1)(ResourceLoadingType, string) | Initializes a new instance of the `StreamProviderOptions` class. |

## Properties

| Name | Description |
| --- | --- |
| [CustomPath](../../aspose.cells/streamprovideroptions/custompath/) { get; set; } | The user custom path(URL) saved in generated html file for the referred source. If not defined by user, DefaultPath will be used. For example, the sheet data will be saved by user to d:/sheet001.htm, the url used in the main html file should be "d:/sheet001.htm" or other valid relative path that can be accessed by the main html file. |
| [DefaultPath](../../aspose.cells/streamprovideroptions/defaultpath/) { get; } | The default path(URL) saved in generated html file for the referred source. For example, the sheet data saved in xxx_files/sheet001.htm, the url used in the main html file should be like "src="xxx_files/sheet001.htm"" |
| [ResourceLoadingType](../../aspose.cells/streamprovideroptions/resourceloadingtype/) { get; set; } | Gets and sets the type of loading resource. |
| [Stream](../../aspose.cells/streamprovideroptions/stream/) { get; set; } | Gets/Sets the stream |

### Examples

```csharp
// Called: void IStreamProvider.InitStream(StreamProviderOptions options)
void IStreamProvider.Type_StreamProviderOptions(StreamProviderOptions options)
            {
                //WebProxy proxy = new WebProxy(proxyUrl);
                WebRequest request = WebRequest.Create(options.DefaultPath);
                //request.Proxy = proxy;
                WebResponse response = request.GetResponse();

                Stream srcStream = response.GetResponseStream();

                byte[] imageBytes = CopyStreamToByteArray(srcStream);
                options.Stream = new MemoryStream(imageBytes);
                ;
            }
```

### See Also

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


