##PivotField.ShowAllItems
PivotField property. Indicates whether all items displays in the PivotTable report even if they dont contain summary data. show items with no data The default value is false
## PivotField.ShowAllItems property
Indicates whether all items displays in the PivotTable report, even if they don't contain summary data. show items with no data The default value is false.
```csharp
public bool ShowAllItems { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyShowAllItemsDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Sample data for pivot table
sheet.Cells["A1"].PutValue("Category");
sheet.Cells["B1"].PutValue("Product");
sheet.Cells["C1"].PutValue("Sales");
sheet.Cells["A2"].PutValue("Electronics");
sheet.Cells["B2"].PutValue("Laptop");
sheet.Cells["C2"].PutValue(1200);
sheet.Cells["A3"].PutValue("Electronics");
sheet.Cells["B3"].PutValue("Phone");
sheet.Cells["C3"].PutValue(800);
sheet.Cells["A4"].PutValue("Furniture");
sheet.Cells["B4"].PutValue("Chair");
sheet.Cells["C4"].PutValue(150);
// Add pivot table
int index = sheet.PivotTables.Add("A1:C4", "E3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Set ShowAllItems property for the row field
PivotField rowField = pivotTable.RowFields[0];
rowField.ShowAllItems = true;
// Calculate data and save
pivotTable.CalculateData();
workbook.Save("PivotFieldShowAllItemsDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
