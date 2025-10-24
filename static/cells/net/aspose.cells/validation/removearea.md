##Validation.RemoveArea
Validation method. Remove the validation settings in the range
## Validation.RemoveArea method
Remove the validation settings in the range.
```csharp
public void RemoveArea(CellArea cellArea)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | the areas where this validation settings should be removed. |
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationMethodRemoveAreaWithCellAreaDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add a validation to the worksheet
Validation validation = worksheet.Validations[worksheet.Validations.Add()];
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "10";
validation.Formula2 = "100";
// Add initial validation area
CellArea initialArea = CellArea.CreateCellArea(0, 0, 0, 0);
validation.AddArea(initialArea);
// Add another area to the validation
CellArea additionalArea = CellArea.CreateCellArea(1, 1, 1, 1);
validation.AddArea(additionalArea);
Console.WriteLine("Validation areas count after adding: " + validation.Areas.Length);
// Remove the additional area
validation.RemoveArea(additionalArea);
Console.WriteLine("Validation areas count after removing: " + validation.Areas.Length);
// Add multiple areas
CellArea[] multipleAreas = new CellArea[]
{
CellArea.CreateCellArea(2, 2, 2, 2),
CellArea.CreateCellArea(3, 3, 3, 3),
CellArea.CreateCellArea(4, 4, 4, 4)
};
validation.AddAreas(multipleAreas, false, false);
Console.WriteLine("Validation areas count after adding multiple: " + validation.Areas.Length);
// Remove one of the areas
validation.RemoveArea(multipleAreas[1]);
Console.WriteLine("Validation areas count after removing one: " + validation.Areas.Length);
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
