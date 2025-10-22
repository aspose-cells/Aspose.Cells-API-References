##PivotTable.ManualUpdate
PivotTable property. Indicates whether the PivotTable report is recalculated only at the users request
## PivotTable.ManualUpdate property
Indicates whether the PivotTable report is recalculated only at the user's request.
```csharp
public bool ManualUpdate { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyManualUpdateDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
// Add a worksheet and populate with sample data
Worksheet dataSheet = workbook.Worksheets["Sheet1"];
dataSheet.Cells["A1"].PutValue("Category");
dataSheet.Cells["B1"].PutValue("Value");
dataSheet.Cells["A2"].PutValue("A");
dataSheet.Cells["B2"].PutValue(10);
dataSheet.Cells["A3"].PutValue("B");
dataSheet.Cells["B3"].PutValue(20);
dataSheet.Cells["A4"].PutValue("A");
dataSheet.Cells["B4"].PutValue(30);
// Add a pivot table
Worksheet pivotSheet = workbook.Worksheets.Add("PivotSheet");
int index = pivotSheet.PivotTables.Add("Sheet1!A1:B4", "A3", "PivotTable1");
PivotTable pivotTable = pivotSheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Enable manual update
pivotTable.ManualUpdate = true;
// At this point, the pivot table won't refresh automatically
Console.WriteLine("Pivot table before refresh (ManualUpdate=true):");
Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will be empty
// Manually refresh the pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
Console.WriteLine("Pivot table after manual refresh:");
Console.WriteLine(pivotSheet.Cells["B4"].StringValue); // Will show "40" (sum of category A)
// Save the workbook
workbook.Save("PivotTableManualUpdateDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
