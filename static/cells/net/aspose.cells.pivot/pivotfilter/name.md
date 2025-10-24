##PivotFilter.Name
PivotFilter property. Gets the name of the pivot filter
## PivotFilter.Name property
Gets the name of the pivot filter.
```csharp
public string Name { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyNameDemo
{
public static void Run()
{
// Create a new workbook
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
// Populate the worksheet with sample data
cells["A1"].Value = "Product";
cells["A2"].Value = "Apple";
cells["A3"].Value = "Banana";
cells["A4"].Value = "Orange";
cells["B1"].Value = "Sales";
cells["B2"].Value = 100;
cells["B3"].Value = 200;
cells["B4"].Value = 300;
// Add a pivot table
PivotTableCollection pivots = sheet.PivotTables;
int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Product");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
// Add and configure a pivot filter
int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[filterIndex];
filter.Name = "ProductFilter"; // Demonstrating Name property usage
filter.AutoFilter.FilterTop10(0, false, false, 2);
// Refresh and calculate pivot data
pivot.RefreshData();
pivot.CalculateData();
// Save the workbook
book.Save("PivotFilterNameDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
