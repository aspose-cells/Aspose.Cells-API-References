##PivotFilter.Value1
PivotFilter property. Gets the string value1 of the label pivot filter
## PivotFilter.Value1 property
Gets the string value1 of the label pivot filter.
```csharp
public string Value1 { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyValue1Demo
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
cells["B2"].Value = 1000;
cells["B3"].Value = 2000;
cells["B4"].Value = 3000;
// Add a pivot table
PivotTableCollection pivots = sheet.PivotTables;
int pivotIndex = pivots.Add("=Sheet1!A1:B4", "D1", "SalesPivot");
PivotTable pivot = pivots[pivotIndex];
pivot.AddFieldToArea(PivotFieldType.Row, "Product");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
// Add a pivot filter and set Value1
int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
PivotFilter filter = pivot.PivotFilters[filterIndex];
filter.Value1 = "Apple"; // Filter for Apple products only
// Refresh and calculate data
pivot.RefreshData();
pivot.CalculateData();
// Save the workbook
book.Save("PivotFilterValue1Demo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
