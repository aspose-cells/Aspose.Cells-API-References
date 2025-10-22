##PivotTable.EnableDrilldown
PivotTable property. Gets whether drilldown is enabled
## PivotTable.EnableDrilldown property
Gets whether drilldown is enabled.
```csharp
public bool EnableDrilldown { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyEnableDrilldownDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and populate with sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 150;
worksheet.Cells["B4"].Value = 200;
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Configure pivot table fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Enable drilldown functionality
pivotTable.EnableDrilldown = true;
// Save the workbook
workbook.Save("PivotTableEnableDrilldownDemo.xlsx");
// Verify the property was set
Console.WriteLine("EnableDrilldown property is set to: " + pivotTable.EnableDrilldown);
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
