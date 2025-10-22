##Picture.Formula
Picture property. Gets and sets the data of the formula
## Picture.Formula property
Gets and sets the data of the formula.
```csharp
public string Formula { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class PicturePropertyFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[pictureIndex];
// Set formula for the picture
picture.Formula = "A1:A3";
Console.WriteLine("Picture Formula: " + picture.Formula);
// Change the formula
picture.Formula = "B1:B3";
Console.WriteLine("Updated Picture Formula: " + picture.Formula);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)
