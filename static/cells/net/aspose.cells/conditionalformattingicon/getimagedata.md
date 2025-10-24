##ConditionalFormattingIcon.GetImageData
ConditionalFormattingIcon method. Gets the image data with the setting of cell
## ConditionalFormattingIcon.GetImageData method
Gets the image data with the setting of cell.
```csharp
public byte[] GetImageData(Cell cell)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cell | Cell | The setting of cell. |
### Return Value
Returns the image data of icon.
### Examples
```csharp
using System.IO;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ConditionalFormattingIconMethodGetImageDataWithCellDemo
{
public static void Run()
{
string outputDir = "Output/";
Directory.CreateDirectory(outputDir);
Workbook workbook = new Workbook("example.xlsx");
Worksheet worksheet = workbook.Worksheets[0];
ConditionalFormattingIcon icon = worksheet.ConditionalFormattings[0][0].IconSet.CfIcons[0];
Cell targetCell = worksheet.Cells["E1"];
byte[] imageData = icon.GetImageData(targetCell);
File.WriteAllBytes(Path.Combine(outputDir, "E1_icon.png"), imageData);
targetCell = worksheet.Cells["G1"];
imageData = icon.GetImageData(targetCell);
File.WriteAllBytes(Path.Combine(outputDir, "G1_icon.png"), imageData);
}
}
}
```
### See Also
* class [Cell](../../cell/)
* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
