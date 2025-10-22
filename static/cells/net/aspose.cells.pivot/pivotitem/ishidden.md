##PivotItem.IsHidden
PivotItem property. Gets and Sets whether the pivot item is hidden
## PivotItem.IsHidden property
Gets and Sets whether the pivot item is hidden.
```csharp
public bool IsHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemPropertyIsHiddenDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "债券借贷";
worksheet.Cells["A3"].Value = "股票";
worksheet.Cells["A4"].Value = "基金";
worksheet.Cells["B1"].Value = "Value";
worksheet.Cells["B2"].Value = 1000;
worksheet.Cells["B3"].Value = 2000;
worksheet.Cells["B4"].Value = 3000;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "D3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Access pivot field and items
PivotField field = pivotTable.RowFields[0];
// Set IsHidden property to show only "债券借贷"
foreach (PivotItem item in field.PivotItems)
{
item.IsHidden = (item.Name != "债券借贷");
}
// Refresh pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotItemIsHiddenDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
