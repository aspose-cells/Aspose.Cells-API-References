##PivotFilter.Value2
PivotFilter property. Gets the string value2 of the label pivot filter
## PivotFilter.Value2 property
Gets the string value2 of the label pivot filter.
```csharp
public string Value2 { get; set; }
```
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyValue2Demo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Product";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["A2"].Value = "WidgetA";
worksheet.Cells["B2"].Value = 150;
worksheet.Cells["A3"].Value = "WidgetB";
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["A4"].Value = "WidgetA";
worksheet.Cells["B4"].Value = 75;
int pivotIndex = worksheet.PivotTables.Add("A6", "A1:B4", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Product");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivotTable.PivotFilters[filterIndex];
filter.Value1 = "100";
filter.Value2 = "200";
filter.MeasureFldIndex = 0;
workbook.Save("PivotFilterValue2Demo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
