##Class PivotItemCollection
Aspose.Cells.Pivot.PivotItemCollection class. Represents all the PivotItem objects in the PivotField
## PivotItemCollection class
Represents all the [`PivotItem`](../pivotitem/) objects in the PivotField.
```csharp
public class PivotItemCollection : IEnumerable
```
## Properties
| Name | Description |
| --- | --- |
| [Count](../../aspose.cells.pivot/pivotitemcollection/count/) { get; } | Gets the count of the pivot items. |
| [Item](../../aspose.cells.pivot/pivotitemcollection/item/) { get; } | Gets the PivotItem Object at the specific index. (2 indexers) |
## Methods
| Name | Description |
| --- | --- |
| [ChangeitemsOrder](../../aspose.cells.pivot/pivotitemcollection/changeitemsorder/)(int, int) | (**Obsolete.**) Directly changes the orders of the two items. |
| [GetEnumerator](../../aspose.cells.pivot/pivotitemcollection/getenumerator/)() | Gets an enumerator over the elements in this collection in proper sequence. |
| [SwapItem](../../aspose.cells.pivot/pivotitemcollection/swapitem/)(int, int) | Directly swap two items. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotItemCollectionDemo
{
public static void PivotItemCollectionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells[0, 0].Value = "Fruit";
worksheet.Cells[1, 0].Value = "Apple";
worksheet.Cells[2, 0].Value = "Banana";
worksheet.Cells[3, 0].Value = "Cherry";
worksheet.Cells[4, 0].Value = "Date";
worksheet.Cells[0, 1].Value = "Quantity";
worksheet.Cells[1, 1].Value = 10;
worksheet.Cells[2, 1].Value = 20;
worksheet.Cells[3, 1].Value = 30;
worksheet.Cells[4, 1].Value = 40;
// Add a pivot table to the worksheet
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("=Sheet1!A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity
// Access the PivotField and its PivotItems
PivotField pivotField = pivotTable.RowFields[0];
PivotItemCollection pivotItems = pivotField.PivotItems;
// Display the count of pivot items
Console.WriteLine("Pivot Items Count: " + pivotItems.Count);
// Iterate through the pivot items and display their names
foreach (PivotItem item in pivotItems)
{
Console.WriteLine("Pivot Item: " + item.Name);
}
// Change the order of pivot items
pivotItems.ChangeitemsOrder(0, 2);
// Save the workbook
workbook.Save("PivotItemCollectionExample.xlsx");
return;
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
