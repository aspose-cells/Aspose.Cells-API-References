##WorkbookSettings.ResourceProvider
WorkbookSettings property. Gets and sets the stream provider for external resource such as loading image data for picture of type LinkToFile
## WorkbookSettings.ResourceProvider property
Gets and sets the stream provider for external resource, such as loading image data for picture of type "LinkToFile".
```csharp
public IStreamProvider ResourceProvider { get; set; }
```
### Examples
```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Rendering;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyResourceProviderDemo
{
public static void Run()
{
// Create a sample workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a sample shape to demonstrate resource provider
worksheet.Shapes.AddRectangle(1, 1, 100, 100, 200, 200);
// Set the resource provider
workbook.Settings.ResourceProvider = new MemoryStreamProvider();
// Save the shape as image using the resource provider
string outputPath = "output_shape.png";
worksheet.Shapes[0].ToImage(outputPath, new ImageOrPrintOptions());
Console.WriteLine("Shape saved as image using ResourceProvider.");
}
}
public class MemoryStreamProvider : IStreamProvider
{
public void CloseStream(StreamProviderOptions options)
{
options.Stream.Close();
}
public void InitStream(StreamProviderOptions options)
{
options.Stream = new FileStream(options.DefaultPath, FileMode.Create);
}
}
}
```
### See Also
* interface [IStreamProvider](../../istreamprovider/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
