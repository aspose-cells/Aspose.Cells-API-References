##PivotFilter.EvaluationOrder
PivotFilter property. Gets the Evaluation Order of the pivot filter
## PivotFilter.EvaluationOrder property
Gets the Evaluation Order of the pivot filter.
```csharp
public int EvaluationOrder { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyEvaluationOrderDemo
{
public static void Run()
{
// Create a new workbook
Workbook book = new Workbook();
Worksheet sheet = book.Worksheets[0];
Cells cells = sheet.Cells;
// Populate sample data
cells["A1"].Value = "Category";
cells["A2"].Value = "Fruit";
cells["A3"].Value = "Vegetable";
cells["A4"].Value = "Fruit";
cells["A5"].Value = "Vegetable";
cells["B1"].Value = "Sales";
cells["B2"].Value = 100;
cells["B3"].Value = 200;
cells["B4"].Value = 300;
cells["B5"].Value = 400;
// Create pivot table
PivotTableCollection pivots = sheet.PivotTables;
int pivotIndex = pivots.Add("=Sheet1!A1:B5", "D1", "PivotTable1");
PivotTable pivot = pivots[pivotIndex];
// Add fields
pivot.AddFieldToArea(PivotFieldType.Row, "Category");
pivot.AddFieldToArea(PivotFieldType.Data, "Sales");
// Add pivot filter
int filterIndex = pivot.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivot.PivotFilters[filterIndex];
// Set filter properties including EvaluationOrder
filter.EvaluationOrder = 1;
filter.AutoFilter.FilterTop10(0, false, false, 2);
// Refresh pivot table
pivot.RefreshData();
pivot.CalculateData();
// Save workbook
book.Save("PivotFilterEvaluationOrderDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
