##PivotItemCollection.ChangeitemsOrder
PivotItemCollection method. Directly changes the orders of the two items
## PivotItemCollection.ChangeitemsOrder method
Directly changes the orders of the two items.
```csharp
[Obsolete("Use PivotItemCollection.SwapItem() method instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public void ChangeitemsOrder(int sourceIndex, int destIndex)
```
| Parameter | Type | Description |
| --- | --- | --- |
| sourceIndex | Int32 | The current index |
| destIndex | Int32 | The dest index |
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotItemCollection.SwapItem() method. This method will be removed 12 months later since July 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemCollectionMethodChangeitemsOrderWithInt32Int32Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells[0, 0].Value = "Category";
worksheet.Cells[1, 0].Value = "A";
worksheet.Cells[2, 0].Value = "B";
worksheet.Cells[3, 0].Value = "C";
PivotTableCollection pivotTables = worksheet.PivotTables;
int pivotIndex = pivotTables.Add("=Sheet1!A1:A4", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
PivotField pivotField = pivotTable.RowFields[0];
PivotItemCollection pivotItems = pivotField.PivotItems;
Console.WriteLine("Original Order:");
foreach (PivotItem item in pivotItems)
{
Console.WriteLine(item.Name);
}
pivotItems.ChangeitemsOrder(0, 2);
Console.WriteLine("\nAfter Changing Order:");
foreach (PivotItem item in pivotItems)
{
Console.WriteLine(item.Name);
}
workbook.Save("PivotItemOrderChange.xlsx");
}
}
}
```
### See Also
* class [PivotItemCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
