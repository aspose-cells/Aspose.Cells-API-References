##ValidationCollection.Add
ValidationCollection method. Adds a data validation to the collection
## Add() {#add}
Adds a data validation to the collection.
```csharp
[Obsolete("Use ValidationCollection.Add(CellArea) method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int Add()
```
### Return Value
[`Validation`](../../validation/) object index.
### Remarks
NOTE: This method is now obsolete. Instead, please use ValidationCollection.Add(CellArea) method. This method will be removed 12 months later since JANUARY 2015. Aspose apologizes for any inconvenience you may have experienced.
### See Also
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
## Add(CellArea) {#add_1}
Adds a data validation to the collection.
```csharp
public int Add(CellArea ca)
```
| Parameter | Type | Description |
| --- | --- | --- |
| ca | CellArea | The area contains this validation. |
### Return Value
[`Validation`](../../validation/) object index.
### Examples
```csharp
using System;
using Aspose.Cells;
namespace AsposeCellsExamples
{
public class ValidationCollectionMethodAddWithCellAreaDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Create cell area for validation
CellArea cellarea = new CellArea();
cellarea.StartRow = 0;
cellarea.StartColumn = 0;
cellarea.EndRow = 1;
cellarea.EndColumn = 1;
// Add validation to the collection
int index = sheet.Validations.Add(cellarea);
Validation validation = sheet.Validations[index];
// Configure validation settings
validation.Type = ValidationType.List;
validation.Formula1 = "Yes,No";
validation.AlertStyle = ValidationAlertType.Information;
// Save the workbook
workbook.Save("ValidationCollectionMethodAddWithCellAreaDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* struct [CellArea](../../cellarea/)
* class [ValidationCollection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)
