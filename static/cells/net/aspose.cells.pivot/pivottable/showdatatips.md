##PivotTable.ShowDataTips
PivotTable property. Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells
## PivotTable.ShowDataTips property
Specifies a boolean value that indicates whether tooltips should be displayed for PivotTable data cells.
```csharp
public bool ShowDataTips { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowDataTipsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and some sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["B3"].Value = 15;
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B4"].Value = 20;
// Create a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Configure pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Quantity");
// Enable data tips
pivotTable.ShowDataTips = true;
// Save the workbook
workbook.Save("PivotTableWithDataTips.xlsx");
Console.WriteLine("Pivot table with ShowDataTips enabled created successfully.");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
