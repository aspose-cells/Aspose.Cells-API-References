##Validation.Formula1
Validation property. Represents the value or expression associated with the data validation
## Validation.Formula1 property
Represents the value or expression associated with the data validation.
```csharp
public string Formula1 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyFormula1Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add list validation with Formula1 as comma-separated values
Validation validation1 = worksheet.Validations[worksheet.Validations.Add()];
validation1.Type = ValidationType.List;
validation1.AlertStyle = ValidationAlertType.Stop;
validation1.Formula1 = "A,B,C";
validation1.AddArea(new CellArea() { StartRow = 0, StartColumn = 0, EndRow = 5, EndColumn = 0 });
// Add formula validation with Formula1 as cell reference
Validation validation2 = worksheet.Validations[worksheet.Validations.Add()];
validation2.Type = ValidationType.Custom;
validation2.AlertStyle = ValidationAlertType.Stop;
validation2.Formula1 = "=A5";
validation2.AddArea(new CellArea() { StartRow = 0, StartColumn = 1, EndRow = 5, EndColumn = 1 });
// Save and reload to verify persistence
string outputPath = "output_validation_formula1.xlsx";
workbook.Save(outputPath);
// Reload to verify
Workbook loadedWorkbook = new Workbook(outputPath);
Worksheet loadedSheet = loadedWorkbook.Worksheets[0];
Console.WriteLine("Validation 1 Formula1: " + loadedSheet.Validations[0].Formula1);
Console.WriteLine("Validation 2 Formula1: " + loadedSheet.Validations[1].Formula1);
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
