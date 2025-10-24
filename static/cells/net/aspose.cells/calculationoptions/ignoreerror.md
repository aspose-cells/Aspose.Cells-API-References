##CalculationOptions.IgnoreError
CalculationOptions property. Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function external links etc. The default value is true
## CalculationOptions.IgnoreError property
Indicates whether errors encountered while calculating formulas should be ignored. The error may be unsupported function, external links, etc. The default value is true.
```csharp
public bool IgnoreError { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class CalculationOptionsPropertyIgnoreErrorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a named range that doesn't exist to demonstrate error handling
worksheet.Cells["A1"].Formula = "=NONEXISTENTNAME()";
// Calculate with IgnoreError = false (will throw error)
try
{
workbook.CalculateFormula(new CalculationOptions() { IgnoreError = false });
Console.WriteLine("Calculation completed without ignoring errors");
}
catch (Exception ex)
{
Console.WriteLine("Error occurred (expected): " + ex.Message);
}
// Calculate with IgnoreError = true (will suppress error)
try
{
workbook.CalculateFormula(new CalculationOptions() { IgnoreError = true });
Console.WriteLine("Calculation completed while ignoring errors");
}
catch (Exception ex)
{
Console.WriteLine("Error occurred (unexpected): " + ex.Message);
}
}
}
}
```
### See Also
* class [CalculationOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
