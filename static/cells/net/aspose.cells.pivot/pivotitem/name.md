##PivotItem.Name
PivotItem property. Gets the name of the pivot item
## PivotItem.Name property
Gets the name of the pivot item.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemPropertyNameDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet ws = wb.Worksheets[0];
// Add sample data for pivot table
ws.Cells["A1"].Value = "Category";
ws.Cells["B1"].Value = "Value";
ws.Cells["A2"].Value = "债券借贷";
ws.Cells["A3"].Value = "股票";
ws.Cells["A4"].Value = "基金";
ws.Cells["B2"].Value = 100;
ws.Cells["B3"].Value = 200;
ws.Cells["B4"].Value = 300;
// Create pivot table
int index = ws.PivotTables.Add("A1:B4", "D3", "PivotTable1");
PivotTable pivotTable = ws.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Access pivot items and demonstrate Name property
PivotField field = pivotTable.RowFields[0];
foreach (PivotItem item in field.PivotItems)
{
// Hide all items except "债券借贷"
item.IsHidden = item.Name != "债券借贷";
Console.WriteLine($"Pivot Item Name: {item.Name}, Hidden: {item.IsHidden}");
}
// Refresh and save
pivotTable.RefreshData();
pivotTable.CalculateData();
wb.Save("PivotItemNameDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
