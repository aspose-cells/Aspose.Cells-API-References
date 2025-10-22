##PivotItem.IsDetailHidden
PivotItem property. Gets and sets whether the detail of this pivot item is hidden
## PivotItem.IsDetailHidden property
Gets and sets whether the detail of this pivot item is hidden.
```csharp
public bool IsDetailHidden { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotItemPropertyIsDetailHiddenDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["A2"].PutValue("Fruit");
sheet.Cells["A3"].PutValue("Fruit");
sheet.Cells["A4"].PutValue("Vegetable");
sheet.Cells["A5"].PutValue("Vegetable");
sheet.Cells["B1"].PutValue("Item");
sheet.Cells["B2"].PutValue("Apple");
sheet.Cells["B3"].PutValue("Orange");
sheet.Cells["B4"].PutValue("Carrot");
sheet.Cells["B5"].PutValue("Potato");
sheet.Cells["C1"].PutValue("Amount");
sheet.Cells["C2"].PutValue(10);
sheet.Cells["C3"].PutValue(15);
sheet.Cells["C4"].PutValue(20);
sheet.Cells["C5"].PutValue(25);
// Create pivot table
int index = sheet.PivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row fields
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Item");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Amount");
// Refresh and calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Hide details for "Fruit" category
pivotTable.RowFields[0].PivotItems["Fruit"].IsDetailHidden = true;
// Save the workbook
wb.Save("PivotItemIsDetailHiddenDemo.xlsx");
}
}
}
```
### See Also
* class [PivotItem](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
