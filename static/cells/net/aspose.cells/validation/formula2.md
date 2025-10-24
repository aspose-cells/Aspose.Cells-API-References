##Validation.Formula2
Validation property. Represents the value or expression associated with the data validation
## Validation.Formula2 property
Represents the value or expression associated with the data validation.
```csharp
public string Formula2 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyFormula2Demo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Access first worksheet
Worksheet sheet = workbook.Worksheets[0];
// Add sample data
sheet.Cells["B3"].PutValue(100);
sheet.Cells["B7"].PutValue(50);
// Create validation for cell B7
Validation validation = sheet.Cells["B7"].GetValidation();
// Set validation type and formulas
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "=B3";  // Demonstrating Formula2 usage
// Apply validation
CellArea area = new CellArea();
area.StartRow = 6;
area.StartColumn = 1;
area.EndRow = 6;
area.EndColumn = 1;
validation.AddArea(area);
// Save the workbook
workbook.Save("ValidationFormula2Demo.xlsx");
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
