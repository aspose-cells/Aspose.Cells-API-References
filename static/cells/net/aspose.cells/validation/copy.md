##Validation.Copy
Validation method. Copy validation
## Validation.Copy method
Copy validation.
```csharp
public void Copy(Validation source, CopyOptions copyOption)
```
| Parameter | Type | Description |
| --- | --- | --- |
| source | Validation | The source validation. |
| copyOption | CopyOptions | The copy option. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationMethodCopyWithValidationCopyOptionsDemo
{
public static void Run()
{
// Create a source workbook with sample data and validation
Workbook sourceWorkbook = new Workbook();
Worksheet sourceSheet = sourceWorkbook.Worksheets[0];
// Add sample validation to source sheet
Validation sourceValidation = sourceSheet.Validations[sourceSheet.Validations.Add()];
sourceValidation.Type = ValidationType.WholeNumber;
sourceValidation.Operator = OperatorType.Between;
sourceValidation.Formula1 = "10";
sourceValidation.Formula2 = "20";
// Create CellArea with StartRow, StartColumn, EndRow, EndColumn
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 0;
area.EndColumn = 0;
sourceValidation.AddArea(area);
// Create a destination workbook
Workbook destWorkbook = new Workbook();
Worksheet destSheet = destWorkbook.Worksheets[0];
// Add a validation to destination sheet (will be overwritten by copy)
Validation destValidation = destSheet.Validations[destSheet.Validations.Add()];
destValidation.AddArea(area); // Reuse the same area definition
// Demonstrate Copy method with CopyOptions
CopyOptions options = new CopyOptions();
destValidation.Copy(sourceValidation, options);
// Verify the validation was copied correctly
Console.WriteLine("Validation Type: " + destValidation.Type);
Console.WriteLine("Validation Formula1: " + destValidation.Formula1);
Console.WriteLine("Validation Formula2: " + destValidation.Formula2);
}
}
}
```
### See Also
* class [CopyOptions](../../copyoptions/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
