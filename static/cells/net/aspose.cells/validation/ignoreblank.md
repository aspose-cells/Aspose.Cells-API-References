##Validation.IgnoreBlank
Validation property. Indicates whether blank values are permitted by the range data validation
## Validation.IgnoreBlank property
Indicates whether blank values are permitted by the range data validation.
```csharp
public bool IgnoreBlank { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyIgnoreBlankDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
ValidationCollection validations = sheet.Validations;
CellArea area = new CellArea();
area.StartRow = 0;
area.EndRow = 1;
area.StartColumn = 0;
area.EndColumn = 1;
Validation validation = validations[validations.Add(area)];
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "2";
validation.Formula2 = "20";
validation.IgnoreBlank = true;
Console.WriteLine("Validation created with IgnoreBlank set to: " + validation.IgnoreBlank);
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
