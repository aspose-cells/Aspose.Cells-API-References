##WorkbookSettings.MaxRowsOfSharedFormula
WorkbookSettings property. Gets and sets the max row number of shared formula
## WorkbookSettings.MaxRowsOfSharedFormula property
Gets and sets the max row number of shared formula.
```csharp
public int MaxRowsOfSharedFormula { get; set; }
```
### Remarks
If the number is too large, the autofilter works very slow in MS Excel 2013.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class WorkbookSettingsPropertyMaxRowsOfSharedFormulaDemo
{
public static void Run()
{
Workbook book = new Workbook();
book.Settings.MaxRowsOfSharedFormula = 100;
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
// Set shared formula with 101 rows (exceeds MaxRowsOfSharedFormula)
cells["B1"].SetSharedFormula("=A1", 101, 1);
// Verify formula in last cell
Console.WriteLine("Formula in B101: " + cells["B101"].Formula);
// Increase MaxRowsOfSharedFormula and test again in new sheet
book.Settings.MaxRowsOfSharedFormula = 1024;
Worksheet sheet2 = book.Worksheets.Add("Sheet2");
cells = sheet2.Cells;
cells["B1"].SetSharedFormula("=A1", 101, 1);
Console.WriteLine("Formula in B101 (Sheet2): " + cells["B101"].Formula);
book.Save("output.xlsx");
}
}
}
```
### See Also
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
