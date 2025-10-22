##PivotArea.Filters
PivotArea property. Gets all filters for this PivotArea
## PivotArea.Filters property
Gets all filters for this PivotArea.
```csharp
public PivotAreaFilterCollection Filters { get; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
namespace AsposeCellsExamples
{
public class PivotAreaPropertyFiltersDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet dataSheet = workbook.Worksheets[0];
dataSheet.Name = "SalesData";
// Create sample data
dataSheet.Cells["A1"].PutValue("Category");
dataSheet.Cells["B1"].PutValue("Revenue");
dataSheet.Cells["A2"].PutValue("Electronics");
dataSheet.Cells["B2"].PutValue(1500);
dataSheet.Cells["A3"].PutValue("Furniture");
dataSheet.Cells["B3"].PutValue(800);
dataSheet.Cells["A4"].PutValue("Electronics");
dataSheet.Cells["B4"].PutValue(2200);
// Create pivot table
Worksheet pivotSheet = workbook.Worksheets.Add("PivotReport");
int pivotIndex = pivotSheet.PivotTables.Add("A3", "SalesData!A1:B4", "RevenueAnalysis");
PivotTable pivotTable = pivotSheet.PivotTables[pivotIndex];
// Configure row field with subtotals
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
PivotField rowField = pivotTable.RowFields["Category"];
rowField.IsAutoSubtotals = true;
// Add data field
pivotTable.AddFieldToArea(PivotFieldType.Data, "Revenue");
// Create pivot area and select fields
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.SelectField(PivotFieldType.Data, "Sum of Revenue");
pivotArea.SelectField(PivotFieldType.Row, "Category");
// Demonstrate Filters property usage
Console.WriteLine($"Filter count: {pivotArea.Filters.Count}");
if (pivotArea.Filters.Count > 1)
{
bool hasAutomaticSubtotal = pivotArea.Filters[1].IsSubtotalSet(PivotFieldSubtotalType.Automatic);
Console.WriteLine($"Row field has automatic subtotal: {hasAutomaticSubtotal}");
}
workbook.Save("PivotFiltersDemo.xlsx");
}
}
}
```
### See Also
* class [PivotAreaFilterCollection](../../pivotareafiltercollection/)
* class [PivotArea](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
