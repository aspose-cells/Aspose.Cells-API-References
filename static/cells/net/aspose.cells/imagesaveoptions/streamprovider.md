##ImageSaveOptions.StreamProvider
ImageSaveOptions property. Gets or sets the IStreamProvider for exporting objects
## ImageSaveOptions.StreamProvider property
Gets or sets the IStreamProvider for exporting objects.
```csharp
public IStreamProvider StreamProvider { get; set; }
```
### Remarks
If saving as Tiff, this property is ignored. Otherwise, if more than one image should be saving, we will write other images by this. For advanced usage, please use [`WorkbookRender`](../../../aspose.cells.rendering/workbookrender/) or [`SheetRender`](../../../aspose.cells.rendering/sheetrender/).
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CustomStreamProvider : IStreamProvider
{
private int m_count = 0;
public void InitStream(StreamProviderOptions options)
{
m_count++;
}
public Stream GetStream(StreamProviderOptions options)
{
return new FileStream(options.DefaultPath + m_count + ".png", FileMode.Create);
}
public void CloseStream(StreamProviderOptions options)
{
// Implementation when no stream is provided
}
public void CloseStream(StreamProviderOptions options, Stream stream)
{
stream.Dispose();
}
}
public class ImageSaveOptionsPropertyStreamProviderDemo
{
public static void Run()
{
// Create workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Test StreamProvider");
// Set save options with custom stream provider
ImageSaveOptions saveOptions = new ImageSaveOptions(SaveFormat.Png);
saveOptions.StreamProvider = new CustomStreamProvider();
// Save with stream provider
workbook.Save("output.png", saveOptions);
}
}
}
```
### See Also
* interface [IStreamProvider](../../istreamprovider/)
* class [ImageSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
