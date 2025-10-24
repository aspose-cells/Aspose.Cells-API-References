##Validation.AddAreas
Validation method. Applies the validation to given areas
## Validation.AddAreas method
Applies the validation to given areas.
```csharp
public void AddAreas(CellArea[] areas, bool checkIntersection, bool checkEdge)
```
| Parameter | Type | Description |
| --- | --- | --- |
| areas | CellArea[] | The areas. |
| checkIntersection | Boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that all the added areas do not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | Boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if one of given areas will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that no one of those added areas is the top-left, this parameter can be set as false for performance consideration. |
### Remarks
In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using System;
public class ValidationMethodAddAreasWithCellAreaBooleanBooleanDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
int validationIndex = worksheet.Validations.Add();
Validation validation = worksheet.Validations[validationIndex];
validation.Type = ValidationType.List;
validation.AlertStyle = ValidationAlertType.Stop;
validation.Operator = OperatorType.None;
validation.Formula1 = "1,2,3";
validation.InCellDropDown = true;
CellArea[] areas = new CellArea[2];
areas[0] = new CellArea { StartRow = 0, StartColumn = 0, EndRow = 1, EndColumn = 1 };
areas[1] = new CellArea { StartRow = 2, StartColumn = 2, EndRow = 3, EndColumn = 3 };
try
{
validation.AddAreas(areas, true, false);
Console.WriteLine("Added validation areas with checkIntersection=true, checkEdge=false");
foreach (CellArea area in validation.Areas)
{
Console.WriteLine($"Validation area: R{area.StartRow + 1}C{area.StartColumn + 1}:R{area.EndRow + 1}C{area.EndColumn + 1}");
}
}
catch (Exception ex)
{
Console.WriteLine($"Error adding validation areas: {ex.Message}");
}
workbook.Save("ValidationAddAreasDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
