##PivotTable.IsExcel2003Compatible
PivotTable property. Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable if true a string must be less than or equal to 255 characters so if the string is greater than 255 characters it will be truncated. if false a string will not have the aforementioned restriction. The default value is true
## PivotTable.IsExcel2003Compatible property
Specifies whether the PivotTable is compatible for Excel2003 when refreshing PivotTable, if true, a string must be less than or equal to 255 characters, so if the string is greater than 255 characters, it will be truncated. if false, a string will not have the aforementioned restriction. The default value is true.
```csharp
public bool IsExcel2003Compatible { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyIsExcel2003CompatibleDemo
{
public static void Run()
{
// Create a new workbook
Workbook wb = new Workbook();
// Add a worksheet and populate with sample data
Worksheet dataSheet = wb.Worksheets[0];
dataSheet.Name = "Data";
dataSheet.Cells["A1"].Value = "Product";
dataSheet.Cells["B1"].Value = "Description";
dataSheet.Cells["C1"].Value = "Status";
dataSheet.Cells["D1"].Value = "Date";
// Add sample data rows
dataSheet.Cells["A2"].Value = "Product1";
dataSheet.Cells["B2"].Value = "Short description";
dataSheet.Cells["C2"].Value = "Active";
dataSheet.Cells["D2"].Value = DateTime.Now;
dataSheet.Cells["A3"].Value = "Product2";
dataSheet.Cells["B3"].Value = "Very long description that exceeds Excel 2003 limits when used in pivot tables";
dataSheet.Cells["C3"].Value = "Inactive";
dataSheet.Cells["D3"].Value = DateTime.Now.AddDays(-1);
// Add a pivot table
Worksheet pivotSheet = wb.Worksheets.Add("PivotTable");
int pivotIndex = pivotSheet.PivotTables.Add("PivotTable", "A1:D3", "A4", false);
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
// Configure pivot table fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Product
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Description
// Set compatibility mode
pivotTable.IsExcel2003Compatible = false; // Allow longer text in pivot tables
// Refresh and calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
wb.Save("PivotTableExcel2003CompatibilityDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
