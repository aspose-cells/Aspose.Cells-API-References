##PivotFilter.FieldIndex
PivotFilter property. Gets the index of source field which this pivot filter is applied to
## PivotFilter.FieldIndex property
Gets the index of source field which this pivot filter is applied to.
```csharp
public int FieldIndex { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyFieldIndexDemo
{
public static void Run()
{
// Create a new workbook
Workbook workbook = new Workbook();
Worksheet sheet = workbook.Worksheets[0];
// Add sample data for pivot table
Cells cells = sheet.Cells;
cells["A1"].Value = "Fruit";
cells["B1"].Value = "Quantity";
cells["A2"].Value = "Apple";
cells["B2"].Value = 10;
cells["A3"].Value = "Orange";
cells["B3"].Value = 5;
cells["A4"].Value = "Banana";
cells["B4"].Value = 8;
// Add pivot table
int index = sheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add filter
pivotTable.AddFieldToArea(PivotFieldType.Page, 0);
PivotField pivotField = pivotTable.PageFields[0];
// Create pivot filter collection and add filter
PivotFilterCollection filters = pivotTable.PivotFilters;
int filterIndex = filters.Add(0, PivotFilterType.Count);
PivotFilter filter = filters[filterIndex];
// Demonstrate FieldIndex property
Console.WriteLine("Field Index: " + filter.FieldIndex);
// Save the workbook
workbook.Save("PivotFilterFieldIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
