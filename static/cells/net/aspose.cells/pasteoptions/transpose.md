##PasteOptions.Transpose
PasteOptions property. True to transpose rows and columns when the range is pasted. The default value is False
## PasteOptions.Transpose property
True to transpose rows and columns when the range is pasted. The default value is False.
```csharp
public bool Transpose { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PasteOptionsPropertyTransposeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
Cells cells = worksheet.Cells;
// Create source style and apply to horizontal range
Style style = workbook.CreateStyle();
style.ForegroundColor = Color.Yellow;
style.Pattern = BackgroundType.Solid;
Aspose.Cells.Range sourceRange = cells.CreateRange(0, 0, 1, 4);
sourceRange.SetStyle(style);
// Create paste options with transpose
PasteOptions pasteOptions = new PasteOptions();
pasteOptions.PasteType = PasteType.Formats;
pasteOptions.Transpose = true;
// Copy with transpose to vertical range
Aspose.Cells.Range targetRange = cells.CreateRange(2, 0, 4, 1);
targetRange.Copy(sourceRange, pasteOptions);
// Save the workbook
workbook.Save("TransposeDemo.xlsx");
}
}
}
```
### See Also
* class [PasteOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
