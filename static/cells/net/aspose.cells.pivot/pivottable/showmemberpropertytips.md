##PivotTable.ShowMemberPropertyTips
PivotTable property. Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips
## PivotTable.ShowMemberPropertyTips property
Specifies a boolean value that indicates whether member property information should be omitted from PivotTable tooltips.
```csharp
public bool ShowMemberPropertyTips { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyShowMemberPropertyTipsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["A2"].PutValue("Bike");
worksheet.Cells["A3"].PutValue("Car");
worksheet.Cells["A4"].PutValue("Bike");
worksheet.Cells["A5"].PutValue("Car");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["B4"].PutValue(1500);
worksheet.Cells["B5"].PutValue(2500);
// Create a pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display the current value of ShowMemberPropertyTips
Console.WriteLine("Current ShowMemberPropertyTips value: " + pivotTable.ShowMemberPropertyTips);
// Change the ShowMemberPropertyTips property
pivotTable.ShowMemberPropertyTips = false;
Console.WriteLine("ShowMemberPropertyTips set to: " + pivotTable.ShowMemberPropertyTips);
// Calculate data and refresh the pivot table
pivotTable.CalculateData();
pivotTable.RefreshData();
// Save the workbook
workbook.Save("PivotTablePropertyShowMemberPropertyTipsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
