##Validation.RemoveAreas
Validation method. Removes this validation from given areas
## Validation.RemoveAreas method
Removes this validation from given areas.
```csharp
public void RemoveAreas(CellArea[] areas)
```
| Parameter | Type | Description |
| --- | --- | --- |
| areas | CellArea[] | the areas where this validation settings should be removed. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationMethodRemoveAreasWithCellAreaArrayDemo
{
public static void Run()
{
// Create a new workbook and access first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add data validation to the worksheet
int validationIndex = worksheet.Validations.Add();
Validation validation = worksheet.Validations[validationIndex];
// Configure validation settings
validation.Type = ValidationType.WholeNumber;
validation.Operator = OperatorType.Between;
validation.Formula1 = "1";
validation.Formula2 = "10";
// Create two cell areas for validation
CellArea area1 = new CellArea
{
StartRow = 0,
StartColumn = 0,
EndRow = 1,
EndColumn = 1
};  // A1:B2
CellArea area2 = new CellArea
{
StartRow = 2,
StartColumn = 2,
EndRow = 3,  // Original code had (2,2,1,1) which would be invalid endRow < startRow
EndColumn = 3
};  // C3:D4 (corrected end coordinates)
// Add areas to validation
validation.AddArea(area1);
validation.AddArea(area2);
Console.WriteLine($"Added areas: {validation.Areas.Length}");
try
{
// Create array with one area to remove
CellArea[] removeAreas = { area1 };
// Execute RemoveAreas method
validation.RemoveAreas(removeAreas);
Console.WriteLine($"Remaining areas after removal: {validation.Areas.Length}");
// Display remaining areas coordinates
foreach (CellArea remainingArea in validation.Areas)
{
Console.WriteLine($"Area: {remainingArea.StartRow},{remainingArea.StartColumn} to {remainingArea.EndRow},{remainingArea.EndColumn}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
// Save modified workbook
workbook.Save("ValidationRemoveAreasDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
