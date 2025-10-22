##PivotFilter.FilterCategory
PivotFilter property. Gets the category of this filter
## PivotFilter.FilterCategory property
Gets the category of this filter.
```csharp
public FilterCategory FilterCategory { get; }
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFilterPropertyFilterCategoryDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create sample pivot table data
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "A";
worksheet.Cells["A3"].Value = "B";
worksheet.Cells["A4"].Value = "A";
worksheet.Cells["B1"].Value = "Value";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 300;
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add row field using proper API method
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
// Add data field using proper API method
int dataFieldIndex = pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
PivotField dataField = pivotTable.DataFields[dataFieldIndex];
dataField.Function = ConsolidationFunction.Sum;
dataField.DisplayName = "Total";
// Add caption filter to Category field
int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];
// Display FilterCategory property value
Console.WriteLine("FilterCategory value: " + pivotFilter.FilterCategory);
workbook.Save("FilterCategoryDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error: {ex.Message}");
}
}
}
}
```
### See Also
* enum [FilterCategory](../../../aspose.cells/filtercategory/)
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
