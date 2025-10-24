##Enum FilterCategory
Aspose.Cells.FilterCategory enum. Represents the category of the filter
## FilterCategory enumeration
Represents the category of the filter.
```csharp
public enum FilterCategory
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| None | `0` | No Filter. |
| Label | `1` | Caption Filter. |
| NumberValue | `2` | Number Value Filter. |
| Date | `3` | Date Value Filter. |
| Top10 | `4` | Top10 Value Filter. |
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class CellsClassFilterCategoryDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
CreateSampleData(worksheet);
// Create pivot table
int pivotIndex = worksheet.PivotTables.Add("PivotTable", "A1:C7", "H5");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Configure row fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Region
pivotTable.AddFieldToArea(PivotFieldType.Row, 1); // Product
// Configure data field
pivotTable.AddFieldToArea(PivotFieldType.Data, 2); // Sales
// Add label filter to pivot filters
PivotFilter filter = pivotTable.PivotFilters.AddLabelFilter(0, PivotFilterType.CaptionEqual, "East", null);
// Demonstrate FilterCategory usage
Console.WriteLine("Filter Category: " + filter.FilterCategory);
// Display all filter categories in the pivot table
foreach (PivotFilter pivotFilter in pivotTable.PivotFilters)
{
Console.WriteLine($"Filter Type: {pivotFilter.FilterType}, Category: {pivotFilter.FilterCategory}");
}
// Refresh and calculate pivot table
pivotTable.RefreshData();
pivotTable.CalculateData();
// Save the result
workbook.Save("FilterCategoryDemo.xlsx");
}
private static void CreateSampleData(Worksheet worksheet)
{
// Set sample data headers
worksheet.Cells["A1"].Value = "Region";
worksheet.Cells["B1"].Value = "Product";
worksheet.Cells["C1"].Value = "Sales";
// Add sample data rows
object[,] data = new object[,]
{
{"East", "Apples", 5000},
{"West", "Oranges", 3000},
{"East", "Bananas", 4000},
{"North", "Apples", 6000},
{"South", "Oranges", 2000},
{"East", "Bananas", 4500},
{"West", "Apples", 5500}
};
int rowCount = data.GetLength(0);
int colCount = data.GetLength(1);
for (int i = 0; i < rowCount; i++)
{
for (int j = 0; j < colCount; j++)
{
worksheet.Cells[i + 2, j].Value = data[i, j];
}
}
}
}
}
```
### See Also
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)
