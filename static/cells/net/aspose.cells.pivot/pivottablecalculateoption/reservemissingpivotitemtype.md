##PivotTableCalculateOption.ReserveMissingPivotItemType
PivotTableCalculateOption property. Represents how to reserve missing pivot items
## PivotTableCalculateOption.ReserveMissingPivotItemType property
Represents how to reserve missing pivot items.
```csharp
public ReserveMissingPivotItemType ReserveMissingPivotItemType { get; set; }
```
### Remarks
Only works when [`RefreshData`](../refreshdata/) is true.
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableCalculateOptionPropertyReserveMissingPivotItemTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Sample data
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Value");
sheet.Cells["A2"].PutValue("A");
sheet.Cells["B2"].PutValue(10);
sheet.Cells["A3"].PutValue("B");
sheet.Cells["B3"].PutValue(20);
sheet.Cells["A4"].PutValue("A");
sheet.Cells["B4"].PutValue(30);
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[pivotIndex];
// Configure pivot fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Set calculate options with ReserveMissingPivotItemType
PivotTableCalculateOption options = new PivotTableCalculateOption
{
ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
};
// Calculate with options
pivotTable.CalculateData(options);
// Save result
workbook.Save("PivotTableReserveMissingItemsDemo.xlsx");
}
}
}
```
### See Also
* enum [ReserveMissingPivotItemType](../../reservemissingpivotitemtype/)
* class [PivotTableCalculateOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
