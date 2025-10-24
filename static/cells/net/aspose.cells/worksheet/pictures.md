##Worksheet.Pictures
Worksheet property. Gets a Picture collection
## Worksheet.Pictures property
Gets a [`Picture`](../../../aspose.cells.drawing/picture/) collection.
```csharp
public PictureCollection Pictures { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
namespace AsposeCellsExamples
{
public class WorksheetPropertyPicturesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a picture to the worksheet
int pictureIndex = worksheet.Pictures.Add(0, 0, "example.jpg");
Picture picture = worksheet.Pictures[pictureIndex];
// Set picture properties
picture.Placement = PlacementType.FreeFloating;
picture.BorderLineColor = System.Drawing.Color.Blue;
picture.BorderWeight = 1;
// Save the workbook
workbook.Save("output.xlsx", SaveFormat.Xlsx);
// Load the saved workbook to verify
Workbook loadedWorkbook = new Workbook("output.xlsx");
Console.WriteLine("Number of pictures: " + loadedWorkbook.Worksheets[0].Pictures.Count);
}
}
}
```
### See Also
* class [PictureCollection](../../../aspose.cells.drawing/picturecollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
