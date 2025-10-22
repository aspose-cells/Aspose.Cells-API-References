##CopyOptions.ColumnCharacterWidth
CopyOptions property. Indicates whether copying column width in unit of characters
## CopyOptions.ColumnCharacterWidth property
Indicates whether copying column width in unit of characters.
```csharp
public bool ColumnCharacterWidth { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CopyOptionsPropertyColumnCharacterWidthDemo
{
public static void Run()
{
// Create a source workbook with sample data
Workbook srcWorkbook = new Workbook();
Worksheet srcSheet = srcWorkbook.Worksheets[0];
// Set column width in characters for demonstration
srcSheet.Cells.SetColumnWidth(0, 20); // 20 characters wide
// Add some sample data
srcSheet.Cells["A1"].PutValue("Sample Text");
srcSheet.Cells["A2"].PutValue("Another Sample");
// Create destination workbook
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
// Copy with ColumnCharacterWidth set to true
destSheet.Copy(srcSheet, new CopyOptions()
{
ColumnCharacterWidth = true
});
// Save the result
destWorkbook.Save("output_with_column_width.xlsx", SaveFormat.Xlsx);
// For comparison, copy without ColumnCharacterWidth
Workbook destWorkbook2 = new Workbook();
Worksheet destSheet2 = destWorkbook2.Worksheets[0];
destSheet2.Copy(srcSheet, new CopyOptions()
{
ColumnCharacterWidth = false
});
destWorkbook2.Save("output_without_column_width.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
