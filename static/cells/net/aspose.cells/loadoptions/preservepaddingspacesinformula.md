##LoadOptions.PreservePaddingSpacesInFormula
LoadOptions property. Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false
## LoadOptions.PreservePaddingSpacesInFormula property
Indicates whether preserve those spaces and line breaks that are padded between formula tokens while getting and setting formulas. Default value is false.
```csharp
public bool PreservePaddingSpacesInFormula { get; set; }
```
### Remarks
After loading workbook from template file with this option, [`PreservePaddingSpaces`](../../formulasettings/preservepaddingspaces/) will be set to the same value with this property.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyPreservePaddingSpacesInFormulaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Enable preserving padding spaces in formulas
workbook.Settings.FormulaSettings.PreservePaddingSpaces = true;
// Access first worksheet and set a formula with padding spaces
Worksheet worksheet = workbook.Worksheets[0];
Cell cell = worksheet.Cells["A1"];
string formulaWithSpaces = "= IF(1 <>2, 2, 1)";
cell.Formula = formulaWithSpaces;
// Save and reload the workbook with PreservePaddingSpacesInFormula option
string outputPath = "output.xlsx";
workbook.Save(outputPath, SaveFormat.Xlsx);
LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx)
{
PreservePaddingSpacesInFormula = true
};
Workbook reloadedWorkbook = new Workbook(outputPath, loadOptions);
Worksheet reloadedWorksheet = reloadedWorkbook.Worksheets[0];
// Verify the formula preserved spaces after reloading
Console.WriteLine("Original formula: " + formulaWithSpaces);
Console.WriteLine("Reloaded formula: " + reloadedWorksheet.Cells["A1"].Formula);
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
