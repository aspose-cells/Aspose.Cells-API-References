##CopyOptions.CopyInvalidFormulasAsValues
CopyOptions property. If the formula is not valid for the dest destination only copy values
## CopyOptions.CopyInvalidFormulasAsValues property
If the formula is not valid for the dest destination, only copy values.
```csharp
public bool CopyInvalidFormulasAsValues { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CopyOptionsPropertyCopyInvalidFormulasAsValuesDemo
{
public static void Run()
{
// Create a source workbook with a sample worksheet
Workbook srcWorkbook = new Workbook();
Worksheet srcSheet = srcWorkbook.Worksheets[0];
// Add a formula that might be invalid in some contexts
srcSheet.Cells["A1"].Formula = "=1/0"; // Division by zero - invalid formula
srcSheet.Cells["A2"].Value = "Valid Data";
// Create a destination workbook
Workbook destWorkbook = new Workbook();
// Set copy options to convert invalid formulas to values
CopyOptions copyOptions = new CopyOptions();
copyOptions.CopyInvalidFormulasAsValues = true;
// Copy the worksheet with the options
destWorkbook.Worksheets[0].Copy(srcSheet, copyOptions);
// Verify the results
Console.WriteLine("A1 (invalid formula copied as value): " +
destWorkbook.Worksheets[0].Cells["A1"].Value); // Should show #DIV/0! as value
Console.WriteLine("A2 (valid data): " +
destWorkbook.Worksheets[0].Cells["A2"].Value); // Should show "Valid Data"
}
}
}
```
### See Also
* class [CopyOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
