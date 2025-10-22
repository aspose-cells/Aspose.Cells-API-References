##PivotTableRefreshOption.PivotTableRefreshOption
PivotTableRefreshOption constructor. Represents the options of refreshing data source of the pivot table
## PivotTableRefreshOption constructor
Represents the options of refreshing data source of the pivot table.
```csharp
public PivotTableRefreshOption()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableRefreshOptionMethodCtorDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = worksheet.Cells;
cells["A1"].Value = "Product";
cells["B1"].Value = "Region";
cells["C1"].Value = "Sales";
cells["A2"].Value = "Apple";
cells["B2"].Value = "North";            cells["C2"].Value = 1000;
cells["A3"].Value = "Orange";            cells["B3"].Value = "South";            cells["C3"].Value = 2000;
cells["A4"].Value = "Banana";            cells["B4"].Value = "East";            cells["C4"].Value = 3000;
cells["A5"].Value = "Apple";            cells["B5"].Value = "South";            cells["C5"].Value = 4000;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Region");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Create and configure refresh options using constructor
PivotTableRefreshOption refreshOption = new PivotTableRefreshOption();
refreshOption.ReserveMissingPivotItemType = ReserveMissingPivotItemType.None;
// Refresh pivot table with options
pivotTable.RefreshData(refreshOption);
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableRefreshDemo.xlsx", SaveFormat.Xlsx);
}
}
}
```
### See Also
* class [PivotTableRefreshOption](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
