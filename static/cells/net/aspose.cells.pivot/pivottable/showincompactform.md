##PivotTable.ShowInCompactForm
PivotTable method. Layouts the PivotTable in compact form
## PivotTable.ShowInCompactForm method
Layouts the PivotTable in compact form.
```csharp
public void ShowInCompactForm()
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableMethodShowInCompactFormDemo
{
public static void Run()
{
// Create a workbook from source data
Workbook workbook = new Workbook();
Worksheet sourceSheet = workbook.Worksheets[0];
// Add sample data for pivot table
sourceSheet.Cells["A1"].PutValue("Category");
sourceSheet.Cells["B1"].PutValue("Product");
sourceSheet.Cells["C1"].PutValue("Sales");
sourceSheet.Cells["A2"].PutValue("Electronics");
sourceSheet.Cells["B2"].PutValue("Laptop");
sourceSheet.Cells["C2"].PutValue(1200);
sourceSheet.Cells["A3"].PutValue("Electronics");
sourceSheet.Cells["B3"].PutValue("Phone");
sourceSheet.Cells["C3"].PutValue(800);
sourceSheet.Cells["A4"].PutValue("Furniture");
sourceSheet.Cells["B4"].PutValue("Chair");
sourceSheet.Cells["C4"].PutValue(150);
sourceSheet.Cells["A5"].PutValue("Furniture");
sourceSheet.Cells["B5"].PutValue("Table");
sourceSheet.Cells["C5"].PutValue(300);
// Create a pivot table worksheet
Worksheet pivotSheet = workbook.Worksheets.Add("PivotTable");
// Add pivot table
PivotTableCollection pivotTables = pivotSheet.PivotTables;
int index = pivotTables.Add("=Sheet1!A1:C5", "A3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to areas
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Set the pivot table to show in compact form
pivotTable.ShowInCompactForm();
// Calculate data and refresh
pivotTable.CalculateData();
pivotTable.RefreshData();
// Save the workbook
workbook.Save("PivotTableCompactFormDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
