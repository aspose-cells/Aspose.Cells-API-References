##PivotTable.RefreshDate
PivotTable property. Gets the last date time when the PivotTable was refreshed
## PivotTable.RefreshDate property
Gets the last date time when the PivotTable was refreshed.
```csharp
public DateTime RefreshDate { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyRefreshDateDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 15;
cells["A4"].Value = "Banana";
cells["B4"].Value = 8;
// Add a pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pt = sheet.PivotTables[index];
// Refresh the pivot table to set refresh date
pt.RefreshData();
pt.CalculateData();
// Display refresh date information
Console.WriteLine("Pivot Table Refresh Date: " + pt.RefreshDate.ToLongDateString());
Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);
// Save and reload to demonstrate persistence
string savePath = "PivotTableRefreshDateDemo_Out.xlsx";
wb.Save(savePath);
// Reload and show refresh date again
Workbook wb2 = new Workbook(savePath);
PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
Console.WriteLine("\nAfter reloading:");
Console.WriteLine("Pivot Table Refresh Date: " + pt2.RefreshDate.ToLongDateString());
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
