##Class PivotTableRefreshOption
Aspose.Cells.Pivot.PivotTableRefreshOption class. Represents the options of refreshing data source of the pivot table
## PivotTableRefreshOption class
Represents the options of refreshing data source of the pivot table.
```csharp
public class PivotTableRefreshOption
```
## Constructors
| Name | Description |
| --- | --- |
| [PivotTableRefreshOption](pivottablerefreshoption/)() | Represents the options of refreshing data source of the pivot table. |
## Properties
| Name | Description |
| --- | --- |
| [ReserveMissingPivotItemType](../../aspose.cells.pivot/pivottablerefreshoption/reservemissingpivotitemtype/) { get; set; } | Represents how to reserve missing pivot items. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTableRefreshOptionDemo
{
public static void PivotTableRefreshOptionExample()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add some data to the worksheet
worksheet.Cells[0, 0].Value = "Fruit";
worksheet.Cells[0, 1].Value = "Year";
worksheet.Cells[0, 2].Value = "Amount";
worksheet.Cells[1, 0].Value = "Apple";
worksheet.Cells[1, 1].Value = 2020;
worksheet.Cells[1, 2].Value = 50;
worksheet.Cells[2, 0].Value = "Banana";
worksheet.Cells[2, 1].Value = 2020;
worksheet.Cells[2, 2].Value = 60;
worksheet.Cells[3, 0].Value = "Apple";
worksheet.Cells[3, 1].Value = 2021;
worksheet.Cells[3, 2].Value = 70;
worksheet.Cells[4, 0].Value = "Banana";
worksheet.Cells[4, 1].Value = 2021;
worksheet.Cells[4, 2].Value = 80;
// Add a pivot table to the worksheet
int pivotIndex = worksheet.PivotTables.Add("=Sheet1!A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Column, 1); // Year
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Amount
// Create an instance of PivotTableRefreshOption
PivotTableRefreshOption refreshOption = new PivotTableRefreshOption
{
ReserveMissingPivotItemType = ReserveMissingPivotItemType.All
};
// Refresh the pivot table with the specified options
pivotTable.RefreshData(refreshOption);
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableRefreshOptionExample.xlsx");
}
}
}
```
### See Also
* namespace [Aspose.Cells.Pivot](../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../)
