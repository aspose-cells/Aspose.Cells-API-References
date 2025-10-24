##CellRichValue.Image
CellRichValue property. Gets the image data of the cell
## CellRichValue.Image property
Gets the image data of the cell.
```csharp
public virtual byte[] Image { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System;
using System.IO;
public class CellRichValuePropertyImageDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add an image to worksheet
int index = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[index];
// Get cell rich value containing the image
Cell cell = worksheet.Cells[0, 0];
cell.PutValue("test data");
cell.EmbeddedImage = picture.Data;
// Access the rich value
CellRichValue richValue = cell.GetRichValue();
// Display image properties
Console.WriteLine("Image data length: " + (richValue.Image?.Length ?? 0));
Console.WriteLine("Alt text: " + richValue.AltText);
// Set new alt text for the image
richValue.AltText = "Sample product image";
// Save the workbook
workbook.Save("CellRichValueImageDemo.xlsx");
}
}
}
```
### See Also
* class [CellRichValue](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
