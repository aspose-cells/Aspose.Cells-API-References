##PivotFilter.MeasureFldIndex
PivotFilter property. Gets the measure field index of the pivot filter
## PivotFilter.MeasureFldIndex property
Gets the measure field index of the pivot filter.
```csharp
[Obsolete("Use PivotFilter.ValueFieldIndex property.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public int MeasureFldIndex { get; set; }
```
### Remarks
NOTE: This method is now obsolete. Instead, please use PivotFilter.ValueFieldIndex property. This method will be removed 12 months later since November 2024. Aspose apologizes for any inconvenience you may have experienced.
### Examples
```csharp
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyMeasureFldIndexDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Banana";
worksheet.Cells["A4"].Value = "Apple";
worksheet.Cells["A5"].Value = "Orange";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 300;
worksheet.Cells["B5"].Value = 400;
// Get pivot table collection and add pivot table
int pivotIndex = worksheet.PivotTables.Add("A1:B5", "D1", "PivotTable");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
pivotTable.AddFieldToArea(PivotFieldType.Row, "Fruit");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
pivotTable.AddFieldToArea(PivotFieldType.Data, "Sales");
// Get filter collection and add filter
int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivotTable.PivotFilters[filterIndex];
filter.MeasureFldIndex = 1;
workbook.Save("PivotFilterMeasureFldIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
