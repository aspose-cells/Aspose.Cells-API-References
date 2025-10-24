##Class PivotItem
Aspose.Cells.Pivot.PivotItem class. Represents a item in a PivotField report
## PivotItem class
Represents a item in a PivotField report.
```csharp
public class PivotItem
```
## Properties
| Name | Description |
| --- | --- |
| [Index](../../aspose.cells.pivot/pivotitem/index/) { get; set; } | Gets the index of the pivot item in cache field. |
| [IsCalculatedItem](../../aspose.cells.pivot/pivotitem/iscalculateditem/) { get; } | Indicates whether this pivot item is a calculated formula item. |
| [IsDetailHidden](../../aspose.cells.pivot/pivotitem/isdetailhidden/) { get; set; } | Gets and sets whether the detail of this pivot item is hidden. |
| [IsFormula](../../aspose.cells.pivot/pivotitem/isformula/) { get; set; } | (**Obsolete.**) Indicates whether this pivot item is a calculated formula item. |
| [IsHidden](../../aspose.cells.pivot/pivotitem/ishidden/) { get; set; } | Gets and Sets whether the pivot item is hidden. |
| [IsHideDetail](../../aspose.cells.pivot/pivotitem/ishidedetail/) { get; set; } | (**Obsolete.**) Gets and sets whether the pivot item hides detail. |
| [IsMissing](../../aspose.cells.pivot/pivotitem/ismissing/) { get; } | Indicates whether the item is removed from the data source. |
| [Name](../../aspose.cells.pivot/pivotitem/name/) { get; set; } | Gets the name of the pivot item. |
| [Position](../../aspose.cells.pivot/pivotitem/position/) { get; set; } | Specifying the position index in all the PivotItems,not the PivotItems under the same parent node. |
| [PositionInSameParentNode](../../aspose.cells.pivot/pivotitem/positioninsameparentnode/) { get; set; } | Specifying the position index in the PivotItems under the same parent node. |
| [Value](../../aspose.cells.pivot/pivotitem/value/) { get; } | Gets the value of the pivot item |
## Methods
| Name | Description |
| --- | --- |
| [GetDateTimeValue](../../aspose.cells.pivot/pivotitem/getdatetimevalue/)() | Gets the date time value of the pivot item If the value is null ,it will return DateTime.MinValue |
| [GetDoubleValue](../../aspose.cells.pivot/pivotitem/getdoublevalue/)() | Gets the double value of the pivot item If the value is null or not number ,it will return 0 |
| [GetFormula](../../aspose.cells.pivot/pivotitem/getformula/)() | Gets the formula of this calculated item. Only works when this item is calculated item. |
| [GetStringValue](../../aspose.cells.pivot/pivotitem/getstringvalue/)() | Gets the string value of the pivot item If the value is null, it will return "" |
| [Move](../../aspose.cells.pivot/pivotitem/move/)(int, bool) | Moves the item up or down |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotItemDemo
{
public static void PivotItemExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruit");
worksheet.Cells["A3"].PutValue("Vegetable");
worksheet.Cells["B1"].PutValue("Amount");
worksheet.Cells["B2"].PutValue(50);
worksheet.Cells["B3"].PutValue(30);
// Add a pivot table to the worksheet
int pivotIndex = worksheet.PivotTables.Add("=A1:B3", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Access the pivot items
PivotField pivotField = pivotTable.RowFields[0];
PivotItemCollection pivotItems = pivotField.PivotItems;
int pivotItemCount = pivotItems.Count;
Console.WriteLine("Number of Pivot Items: " + pivotItemCount);
for(int i = 0; i < pivotItemCount; i++)
{
PivotItem pivotItem = pivotItems[i];
// Print the name of the pivot item
Console.WriteLine("Pivot Item Name: " + pivotItem.Name);
// Set properties
pivotItem.IsHidden = false;
pivotItem.Position = 1;
pivotItem.IsHideDetail = false;
// Print the value of the pivot item
Console.WriteLine("Pivot Item Value: " + pivotItem.Value);
// Use methods
string stringValue = pivotItem.GetStringValue();
double doubleValue = pivotItem.GetDoubleValue();
DateTime dateTimeValue = pivotItem.GetDateTimeValue();
Console.WriteLine("String Value: " + stringValue);
Console.WriteLine("Double Value: " + doubleValue);
Console.WriteLine("DateTime Value: " + dateTimeValue);
}
// Save the workbook
workbook.Save("PivotItemExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
