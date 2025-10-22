##PivotAreaFilterCollection.Item
PivotAreaFilterCollection property. Gets filter from the list by the index
## PivotAreaFilterCollection indexer
Gets filter from the list by the index.
```csharp
public PivotAreaFilter this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The Index |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotAreaFilterCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data
worksheet.Cells["A1"].PutValue("Category");
worksheet.Cells["B1"].PutValue("Value");
worksheet.Cells["A2"].PutValue("A");
worksheet.Cells["B2"].PutValue(10);
worksheet.Cells["A3"].PutValue("B");
worksheet.Cells["B3"].PutValue(20);
worksheet.Cells["A4"].PutValue("A");
worksheet.Cells["B4"].PutValue(30);
// Add pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Add fields to pivot areas
pivotTable.AddFieldToArea(PivotFieldType.Row, "Category");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Value");
// Create conditional format
PivotConditionalFormat pcf = pivotTable.ConditionalFormats[pivotTable.ConditionalFormats.Add()];
pcf.ScopeType = PivotConditionFormatScopeType.Field;
// Create pivot area and add filters
PivotArea pivotArea = new PivotArea(pivotTable);
pivotArea.SelectField(PivotFieldType.Data, "Value");
pcf.PivotAreas.Add(pivotArea);
// Demonstrate Item property usage
PivotAreaFilter filter = pivotArea.Filters[0];
filter.IsSubtotalSet(PivotFieldSubtotalType.Automatic);
// Save the workbook
workbook.Save("PivotAreaFilterCollectionPropertyItemDemo.xlsx");
}
}
}
```
### See Also
* class [PivotAreaFilter](../../pivotareafilter/)
* class [PivotAreaFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
