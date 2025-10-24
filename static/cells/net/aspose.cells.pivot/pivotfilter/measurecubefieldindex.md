##PivotFilter.MeasureCubeFieldIndex
PivotFilter property. Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply
## PivotFilter.MeasureCubeFieldIndex property
Specifies the index of the measure cube field. this property is used only by filters in OLAP pivots and specifies on which measure a value filter should apply.
```csharp
public int MeasureCubeFieldIndex { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyMeasureCubeFieldIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
// Add a worksheet and populate with sample data
Worksheet worksheet = workbook.Worksheets[0];
worksheet.Cells["A1"].PutValue("Product");
worksheet.Cells["B1"].PutValue("Sales");
worksheet.Cells["A2"].PutValue("Apple");
worksheet.Cells["B2"].PutValue(1000);
worksheet.Cells["A3"].PutValue("Banana");
worksheet.Cells["B3"].PutValue(2000);
worksheet.Cells["A4"].PutValue("Orange");
worksheet.Cells["B4"].PutValue(3000);
// Add a pivot table
int index = worksheet.PivotTables.Add("A1:B4", "E3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add row and data fields
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Refresh pivot table data
pivotTable.RefreshData();
pivotTable.CalculateData();
// Add a filter to the pivot table
pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
PivotField field = pivotTable.BaseFields[0];
// Create and add filter through PivotTable instead of PivotField
int filterIndex = pivotTable.PivotFilters.Add(field.Position, PivotFilterType.Count);
PivotFilter filter = pivotTable.PivotFilters[filterIndex];
// Display MeasureCubeFieldIndex
Console.WriteLine("MeasureCubeFieldIndex: " + filter.MeasureCubeFieldIndex);
// Save the workbook
workbook.Save("PivotFilterMeasureCubeFieldIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
