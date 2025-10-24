##PivotTable.ShowDrill
PivotTable property. Gets and sets whether showing expand/collapse buttons
## PivotTable.ShowDrill property
Gets and sets whether showing expand/collapse buttons.
```csharp
public bool ShowDrill { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowDrillDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and populate with sample data
Worksheet sheet = workbook.Worksheets[0];
sheet.Name = "Pivot";
sheet.Cells["A1"].Value = "Category";
sheet.Cells["B1"].Value = "Value";
sheet.Cells["A2"].Value = "A";
sheet.Cells["B2"].Value = 100;
sheet.Cells["A3"].Value = "B";
sheet.Cells["B3"].Value = 200;
sheet.Cells["A4"].Value = "A";
sheet.Cells["B4"].Value = 150;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Enable drilldown and show drill indicators
pivotTable.EnableDrilldown = true;
pivotTable.ShowDrill = true;
// Refresh and calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableShowDrillDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
