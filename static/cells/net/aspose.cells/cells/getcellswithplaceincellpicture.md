##Cells.GetCellsWithPlaceInCellPicture
Cells method. Gets all cells that contain embedded picture
## Cells.GetCellsWithPlaceInCellPicture method
Gets all cells that contain embedded picture.
```csharp
public IEnumerator GetCellsWithPlaceInCellPicture()
```
### Return Value
Enumerator to enumerate all Cell objects that contain embedded picture
### Remarks
If there is no picture which is set as "Place in Cell" in this worksheet, null will be returned.
### Examples
```csharp
using System;
using System.IO;
using System.Collections;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CellsMethodGetCellsWithPlaceInCellPictureDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add a picture to worksheet (this won't be counted by GetCellsWithPlaceInCellPicture)
workbook.Worksheets[0].Pictures.Add(0, 0, "sample.png");
// Add an embedded image to cell B3 (this will be counted)
workbook.Worksheets[0].Cells["B3"].EmbeddedImage = File.ReadAllBytes("sample.png");
// Remove the floating picture
workbook.Worksheets[0].Pictures.RemoveAt(0);
// Get cells with embedded images
Cells cells = workbook.Worksheets[0].Cells;
int count = 0;
IEnumerator enumerator = cells.GetCellsWithPlaceInCellPicture();
while (enumerator.MoveNext())
{
Cell cell = (Cell)enumerator.Current;
byte[] imageData = cell.EmbeddedImage;
if (imageData != null)
{
count++;
Console.WriteLine($"Found image in cell {cell.Name}");
}
}
Console.WriteLine($"Total cells with embedded images: {count}");
// Save and reload to verify persistence
workbook.Save("output.xlsx");
workbook = new Workbook("output.xlsx");
// Verify after reload
cells = workbook.Worksheets[0].Cells;
count = 0;
enumerator = cells.GetCellsWithPlaceInCellPicture();
while (enumerator.MoveNext())
{
Cell cell = (Cell)enumerator.Current;
byte[] imageData = cell.EmbeddedImage;
if (imageData != null)
{
count++;
}
}
Console.WriteLine($"After reload - cells with embedded images: {count}");
}
}
}
```
### See Also
* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
