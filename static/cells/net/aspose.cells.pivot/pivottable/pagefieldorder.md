##PivotTable.PageFieldOrder
PivotTable property. Gets and sets the order in which page fields are added to the PivotTable reports layout
## PivotTable.PageFieldOrder property
Gets and sets the order in which page fields are added to the PivotTable report's layout.
```csharp
public PrintOrderType PageFieldOrder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyPageFieldOrderDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
var cells = worksheet.Cells;
cells["A1"].Value = "Category";
cells["B1"].Value = "Product";
cells["C1"].Value = "Region";
cells["D1"].Value = "Sales";
// Add sample data rows
for (int i = 2; i <= 10; i++)
{
cells[$"A{i}"].Value = $"Category{(i % 3) + 1}";
cells[$"B{i}"].Value = $"Product{(i % 4) + 1}";
cells[$"C{i}"].Value = $"Region{(i % 2) + 1}";
cells[$"D{i}"].Value = i * 100;
}
// Create pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:D11", "F5", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to areas
pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Category"]);
pivotTable.AddFieldToArea(PivotFieldType.Page, pivotTable.BaseFields["Region"]);
pivotTable.AddFieldToArea(PivotFieldType.Row, pivotTable.BaseFields["Product"]);
pivotTable.AddFieldToArea(PivotFieldType.Data, pivotTable.BaseFields["Sales"]);
// Set page field order and wrap count
pivotTable.PageFieldOrder = PrintOrderType.DownThenOver;
pivotTable.PageFieldWrapCount = 2;
// Save the workbook
workbook.Save("PivotTablePageFieldOrderDemo_out.xlsx");
}
}
}
```
### See Also
* enum [PrintOrderType](../../../aspose.cells/printordertype/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
