##PivotTable.ShowPivotStyleRowStripes
PivotTable property. Indicates whether row stripe formatting is applied
## PivotTable.ShowPivotStyleRowStripes property
Indicates whether row stripe formatting is applied.
```csharp
public bool ShowPivotStyleRowStripes { get; set; }
```
### Examples
```csharp
using System;
using System.Data;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyShowPivotStyleRowStripesDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Create sample data
DataTable data = new DataTable();
data.Columns.Add("Category", typeof(string));
data.Columns.Add("Product", typeof(string));
data.Columns.Add("Sales", typeof(int));
data.Rows.Add("Electronics", "Laptop", 1200);
data.Rows.Add("Electronics", "Phone", 800);
data.Rows.Add("Clothing", "Shirt", 50);
data.Rows.Add("Clothing", "Pants", 70);
data.Rows.Add("Furniture", "Chair", 150);
data.Rows.Add("Furniture", "Table", 300);
// Import data to worksheet
worksheet.Cells.ImportData(data, 0, 0, new ImportTableOptions());
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:C7", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add rows and columns
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Category
pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
// Enable row stripes
pivotTable.ShowPivotStyleRowStripes = true;
// Calculate data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTableWithRowStripes.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
