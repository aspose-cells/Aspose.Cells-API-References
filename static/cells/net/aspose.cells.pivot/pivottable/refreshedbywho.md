##PivotTable.RefreshedByWho
PivotTable property. Gets the name of the last user who refreshed this PivotTable
## PivotTable.RefreshedByWho property
Gets the name of the last user who refreshed this PivotTable
```csharp
public string RefreshedByWho { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyRefreshedByWhoDemo
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
// Create pivot table
int pivotIndex = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pt = sheet.PivotTables[pivotIndex];
// Add fields to pivot table
pt.AddFieldToArea(PivotFieldType.Row, 0);
pt.AddFieldToArea(PivotFieldType.Data, 1);
// Refresh pivot table to set RefreshedByWho property
pt.RefreshData();
pt.CalculateData();
// Output refresh information
Console.WriteLine("Pivot Table Refresh Information:");
Console.WriteLine("Last Refresh Date: " + pt.RefreshDate);
Console.WriteLine("Refreshed By: " + pt.RefreshedByWho);
// Save and reload to demonstrate property persistence
string savePath = "PivotTableRefreshedByWhoDemo_Out.xlsx";
wb.Save(savePath);
// Reload the workbook and check the property
Workbook wb2 = new Workbook(savePath);
PivotTable pt2 = wb2.Worksheets[0].PivotTables[0];
Console.WriteLine("\nAfter Reload:");
Console.WriteLine("Last Refresh Date: " + pt2.RefreshDate);
Console.WriteLine("Refreshed By: " + pt2.RefreshedByWho);
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
