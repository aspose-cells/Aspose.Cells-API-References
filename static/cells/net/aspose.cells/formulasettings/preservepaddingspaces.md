##FormulaSettings.PreservePaddingSpaces
FormulaSettings property. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false
## FormulaSettings.PreservePaddingSpaces property
Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.
```csharp
public bool PreservePaddingSpaces { get; set; }
```
### Remarks
Generally those spaces and line breaks are jsut for visual purpose, Preserving them or not does not affect the calculated result. For performance consideration, if there is no special requirement, it is better not to preserve them while processing formulas.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class FormulaSettingsPropertyPreservePaddingSpacesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Set formula with padding spaces
string formulaWithSpaces = "=SUM( IF( A1:A5 > 10, B1:B5, 0 ) )";
worksheet.Cells["C1"].Formula = formulaWithSpaces;
// Default behavior (PreservePaddingSpaces is true)
Console.WriteLine("Formula with spaces preserved: " + worksheet.Cells["C1"].Formula);
// Change setting to remove padding spaces
workbook.Settings.FormulaSettings.PreservePaddingSpaces = false;
worksheet.Cells["C2"].Formula = formulaWithSpaces;
Console.WriteLine("Formula with spaces removed: " + worksheet.Cells["C2"].Formula);
// Save the workbook
workbook.Save("FormulaSpacesDemo.xlsx");
}
}
}
```
### See Also
* class [FormulaSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
