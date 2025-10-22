##SlicerCacheItem.Selected
SlicerCacheItem property. Specifies whether the SlicerItem is selected or not
## SlicerCacheItem.Selected property
Specifies whether the SlicerItem is selected or not.
```csharp
public bool Selected { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using Aspose.Cells.Slicers;
namespace AsposeCellsExamples
{
public class SlicerCacheItemPropertySelectedDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 300;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
pivotTable.RefreshData();
pivotTable.CalculateData();
// Add slicer
int slicerIndex = worksheet.Slicers.Add(pivotTable, "Fruit", "Slicer1");
Aspose.Cells.Slicers.Slicer slicer = worksheet.Slicers[slicerIndex];
slicer.StyleType = SlicerStyleType.SlicerStyleLight1;
// Access slicer cache items
for (int i = 0; i < slicer.SlicerCache.SlicerCacheItems.Count; i++)
{
SlicerCacheItem item = slicer.SlicerCache.SlicerCacheItems[i];
// Select first item, deselect others
if (i == 0)
{
item.Selected = true;
Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
}
else
{
item.Selected = false;
Console.WriteLine($"Item '{item.Value}' is selected: {item.Selected}");
}
}
// Save the workbook
workbook.Save("SlicerCacheItemSelectedDemo.xlsx");
}
}
}
```
### See Also
* class [SlicerCacheItem](../)
* namespace [Aspose.Cells.Slicers](../../../aspose.cells.slicers/)
* assembly [Aspose.Cells](../../../)
