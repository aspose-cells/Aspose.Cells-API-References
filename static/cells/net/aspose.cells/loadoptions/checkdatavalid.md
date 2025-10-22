##LoadOptions.CheckDataValid
LoadOptions property. Check whether data is valid in the template file
## LoadOptions.CheckDataValid property
Check whether data is valid in the template file.
```csharp
public bool CheckDataValid { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class LoadOptionsPropertyCheckDataValidDemo
{
public static void Run()
{
// Create load options with CheckDataValid set to false
LoadOptions options = new LoadOptions(LoadFormat.Xlsx);
options.CheckDataValid = false;
// Load workbook with these options
Workbook workbook = new Workbook("example.xlsx", options);
// Access first worksheet
Worksheet worksheet = workbook.Worksheets[0];
// Add some data validation for demonstration
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "100";
// Set validation range
CellArea area = new CellArea();
area.StartRow = 0;
area.StartColumn = 0;
area.EndRow = 10;
area.EndColumn = 0;
validation.AddArea(area);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
