##PivotField.ItemCount
PivotField property. Gets the count of the base items in this pivot field
## PivotField.ItemCount property
Gets the count of the base items in this pivot field.
```csharp
public int ItemCount { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldPropertyItemCountDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["A2"].PutValue("Fruit");
worksheet.Cells["A3"].PutValue("Fruit");
worksheet.Cells["A4"].PutValue("Vegetable");
worksheet.Cells["A5"].PutValue("Vegetable");
worksheet.Cells["A6"].PutValue("Fruit");
worksheet.Cells["A7"].PutValue("Vegetable");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["B2"].PutValue(100);
worksheet.Cells["B3"].PutValue(150);
worksheet.Cells["B4"].PutValue(200);
worksheet.Cells["B5"].PutValue(120);
worksheet.Cells["B6"].PutValue(180);
worksheet.Cells["B7"].PutValue(90);
// Add pivot table
int index = worksheet.PivotTables.Add("A1:B7", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row field
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Get the pivot field and display its item count
PivotField pivotField = pivotTable.RowFields[0];
Console.WriteLine("Item count in pivot field: " + pivotField.ItemCount);
// Save the workbook
workbook.Save("PivotFieldItemCountDemo.xlsx");
}
}
}
```
### See Also
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
