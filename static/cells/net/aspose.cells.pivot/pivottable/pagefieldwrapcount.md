##PivotTable.PageFieldWrapCount
PivotTable property. Gets the number of page fields in each column or row in the PivotTable report
## PivotTable.PageFieldWrapCount property
Gets the number of page fields in each column or row in the PivotTable report.
```csharp
public int PageFieldWrapCount { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTablePropertyPageFieldWrapCountDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
// Put in data
Worksheet data = workbook.Worksheets.Add("data");
data.Cells["A1"].PutValue("Country");
data.Cells["B1"].PutValue("Product");
data.Cells["C1"].PutValue("Vendor");
data.Cells["D1"].PutValue("Value");
data.Cells["A2"].PutValue("USA");
data.Cells["B2"].PutValue("Car");
data.Cells["C2"].PutValue("Ford");
data.Cells["D2"].PutValue(1200.987654321);
data.Cells["A3"].PutValue("Japan");
data.Cells["B3"].PutValue("Bike");
data.Cells["C3"].PutValue("Yamaha");
data.Cells["D3"].PutValue(985.123456789);
// Create pivot table
Worksheet pivot = workbook.Worksheets.Add("pivot");
PivotTableCollection pivotTables = pivot.PivotTables;
int index = pivotTables.Add("=data!A1:D3", "A1", "pivotTable1");
PivotTable pivotTable = pivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, "Country");
pivotTable.AddFieldToArea(PivotFieldType.Column, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Page, "Vendor");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Set PageFieldWrapCount property
pivotTable.PageFieldWrapCount = 2; // Number of page fields per row
// Calculate and refresh pivot table
pivotTable.CalculateData();
// Save the workbook
workbook.Save("PivotTablePageFieldWrapCountDemo.xlsx");
}
}
}
```
### See Also
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
