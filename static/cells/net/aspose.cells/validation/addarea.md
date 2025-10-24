##Validation.AddArea
Validation method. Applies the validation to the area
## AddArea(CellArea) {#addarea}
Applies the validation to the area.
```csharp
public void AddArea(CellArea cellArea)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area. |
### Remarks
It is equivalent to use `AddArea` with checking intersection and edge.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationMethodAddAreaWithCellAreaDemo
{
public static void Run()
{
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Create a validation
ValidationCollection vc = sheet.Validations;
Validation validation = vc[vc.Add(CellArea.CreateCellArea(0, 0, 0, 0))];
validation.Type = ValidationType.List;
validation.Formula1 = "=A1:A10";
// Add more areas to the validation
for (int i = 1; i < 5; i++)
{
validation.AddArea(CellArea.CreateCellArea(i, 0, i, 0));
}
// Save the workbook
wb.Save("ValidationMethodAddAreaWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
Console.WriteLine("Validation with multiple areas created successfully.");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## AddArea(CellArea, bool, bool) {#addarea_1}
Applies the validation to the area.
```csharp
public void AddArea(CellArea cellArea, bool checkIntersection, bool checkEdge)
```
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | CellArea | The area. |
| checkIntersection | Boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that the added area does not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | Boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if given area will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that the added area is not the top-left one, this parameter can be set as false for performance consideration. |
### Remarks
In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationMethodAddAreaWithCellAreaBooleanBooleanDemo
{
public static void Run()
{
// Create a workbook and get the first worksheet
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create a validation in a specific area
Validation validation = worksheet.Validations[worksheet.Validations.Add(CellArea.CreateCellArea(5, 3, 6, 3))];
validation.Operator = OperatorType.GreaterThan;
validation.Formula1 = "F3";
// Demonstrate AddArea with CellArea and two boolean parameters
validation.AddArea(CellArea.CreateCellArea(3, 3, 3, 4), false, true);
Console.WriteLine("Area count after AddArea: " + validation.Areas.Length);
Console.WriteLine("Formula1 after AddArea: " + validation.Formula1);
// Remove the added area
validation.RemoveArea(CellArea.CreateCellArea(3, 3, 3, 4));
Console.WriteLine("Area count after RemoveArea: " + validation.Areas.Length);
// Add multiple areas with bulk operation
CellArea[] areas = new CellArea[10];
for (int i = 0; i < areas.Length; i++)
{
areas[i] = CellArea.CreateCellArea(6 + i, 3, 6 + i, 4);
}
validation.AddAreas(areas, true, true);
Console.WriteLine("Area count after bulk AddAreas: " + validation.Areas.Length);
// Save the workbook
workbook.Save("ValidationMethodAddAreaDemo.xlsx");
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [Validation](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
