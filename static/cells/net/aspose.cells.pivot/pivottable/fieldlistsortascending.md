##PivotTable.FieldListSortAscending
PivotTable property. Indicates whether fields in the PivotTable are sorted in nondefault order in the field list
## PivotTable.FieldListSortAscending property
Indicates whether fields in the PivotTable are sorted in non-default order in the field list.
```csharp
public bool FieldListSortAscending { get; set; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotTablePropertyFieldListSortAscendingDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for the pivot table
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["B1"].Value = "Product";
worksheet.Cells["C1"].Value = "Sales";
worksheet.Cells["A2"].Value = "Electronics";
worksheet.Cells["B2"].Value = "Laptop";
worksheet.Cells["C2"].Value = 1200;
worksheet.Cells["A3"].Value = "Electronics";
worksheet.Cells["B3"].Value = "Phone";
worksheet.Cells["C3"].Value = 800;
worksheet.Cells["A4"].Value = "Furniture";
worksheet.Cells["B4"].Value = "Chair";
worksheet.Cells["C4"].Value = 150;
worksheet.Cells["A5"].Value = "Furniture";
worksheet.Cells["B5"].Value = "Table";
worksheet.Cells["C5"].Value = 250;
// Create a pivot table
PivotTableCollection pivotTables = worksheet.PivotTables;
int index = pivotTables.Add("A1:C5", "E3", "PivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Display current FieldListSortAscending value
Console.WriteLine("Initial FieldListSortAscending: " + pivotTable.FieldListSortAscending);
// Show field list in ascending order
pivotTable.FieldListSortAscending = true;
Console.WriteLine("FieldListSortAscending set to: " + pivotTable.FieldListSortAscending);
// Refresh and calculate the pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableFieldListSortAscendingDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
