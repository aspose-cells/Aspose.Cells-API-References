##PasteOptions.IgnoreLinksToOriginalFile
PasteOptions property. Ingore links to the original file
## PasteOptions.IgnoreLinksToOriginalFile property
Ingore links to the original file.
```csharp
public bool IgnoreLinksToOriginalFile { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class PasteOptionsPropertyIgnoreLinksToOriginalFileDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet src = workbook.Worksheets[0];
// Create sample data with formulas that might link to original file
src.Cells["A1"].PutValue("Header1");
src.Cells["B1"].PutValue("Header2");
src.Cells["A2"].PutValue(100);
src.Cells["B2"].PutValue("=A2*2");  // Simple formula
src.Cells["A3"].PutValue(200);
src.Cells["B3"].PutValue("=A3*2");
// Create destination worksheet and range
Worksheet dst = workbook.Worksheets.Add("Destination");
Aspose.Cells.Range srcRange = src.Cells.CreateRange("A1:B3");
Aspose.Cells.Range dstRange = dst.Cells.CreateRange("A1:B3");
// Configure paste options to ignore links to original file
PasteOptions pasteOptions = new PasteOptions();
pasteOptions.PasteType = PasteType.All;
pasteOptions.IgnoreLinksToOriginalFile = true;
// Copy with the specified paste options
dstRange.Copy(srcRange, pasteOptions);
// Save the workbook
workbook.Save("PasteOptions_IgnoreLinksToOriginalFile_Output.xlsx");
}
}
}
```
### See Also
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
