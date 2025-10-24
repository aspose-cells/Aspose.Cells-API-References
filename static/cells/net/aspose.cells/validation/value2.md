##Validation.Value2
Validation property. Represents the second value associated with the data validation
## Validation.Value2 property
Represents the second value associated with the data validation.
```csharp
public object Value2 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationPropertyValue2Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
ValidationCollection validations = worksheet.Validations;
int index = validations.Add(CellArea.CreateCellArea(0, 0, 1, 1));
Validation validation = validations[index];
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "-1000";
validation.Formula2 = "1000";
Console.WriteLine("Validation Value1: " + validation.Value1);
Console.WriteLine("Validation Value2: " + validation.Value2);
}
}
}
```
### See Also
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
