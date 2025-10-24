##PivotTableRefreshOption.ReserveMissingPivotItemType
PivotTableRefreshOption property. Represents how to reserve missing pivot items
## PivotTableRefreshOption.ReserveMissingPivotItemType property
Represents how to reserve missing pivot items.
```csharp
public ReserveMissingPivotItemType ReserveMissingPivotItemType { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableRefreshOptionPropertyReserveMissingPivotItemTypeDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells[0, 0].Value = "Category";
worksheet.Cells[0, 1].Value = "Quarter";
worksheet.Cells[0, 2].Value = "Sales";
worksheet.Cells[1, 0].Value = "Electronics";
worksheet.Cells[1, 1].Value = "Q1";
worksheet.Cells[1, 2].Value = 1000;
worksheet.Cells[2, 0].Value = "Clothing";
worksheet.Cells[2, 1].Value = "Q1";
worksheet.Cells[2, 2].Value = 800;
worksheet.Cells[3, 0].Value = "Electronics";
worksheet.Cells[3, 1].Value = "Q2";
worksheet.Cells[3, 2].Value = 1200;
int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Column, 1);
pivotTable.AddFieldToArea(PivotFieldType.Data, 2);
PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
{
ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
};
pivotTable.RefreshData(refreshOption);
pivotTable.CalculateData();
workbook.Save("PivotTableWithReserveMissingItems.xlsx");
}
}
}
```
### See Also
* enum [ReserveMissingPivotItemType](../../reservemissingpivotitemtype/)
* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
