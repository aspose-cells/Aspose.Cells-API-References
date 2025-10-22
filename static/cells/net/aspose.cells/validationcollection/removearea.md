##ValidationCollection.RemoveArea
ValidationCollection method. Removes all validation setting on the range
## ValidationCollection.RemoveArea method
Removes all validation setting on the range..
```csharp
public void RemoveArea(CellArea ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The range which contains the validations setting. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationCollectionMethodRemoveAreaDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a validation in a specific area
ValidationCollection validations = worksheet.Validations;
CellArea validationArea = CellArea.CreateCellArea(0, 0, 5, 5);
int validationIndex = validations.Add(validationArea);
// Create an area to remove from validation
CellArea removeArea = CellArea.CreateCellArea(2, 2, 4, 4);
try
{
// Call the RemoveArea method with the CellArea parameter
validations.RemoveArea(removeArea);
Console.WriteLine("Validation area removed successfully.");
// Display the remaining validation areas
foreach (Validation validation in validations)
{
if (validation.Areas.Length > 0)
{
Console.WriteLine($"Remaining validation area: {validation.Areas[0]}");
}
}
}
catch (Exception ex)
{
Console.WriteLine($"Error executing RemoveArea method: {ex.Message}");
}
// Save the result
workbook.Save("ValidationRemoveAreaDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
