##PivotField.GetPivotFilterByType
PivotField method. Gets the pivot filter of the pivot field by type
## PivotField.GetPivotFilterByType method
Gets the pivot filter of the pivot field by type
```csharp
public PivotFilter GetPivotFilterByType(PivotFilterType type)
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFieldMethodGetPivotFilterByTypeWithPivotFilterTypeDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook wb = new Workbook();
Worksheet sheet = wb.Worksheets[0];
// Add sample data for pivot table
sheet.Cells["A1"].Value = "Fruit";
sheet.Cells["A2"].Value = "Apple";
sheet.Cells["A3"].Value = "Orange";
sheet.Cells["A4"].Value = "Banana";
sheet.Cells["A5"].Value = "Apple";
sheet.Cells["B1"].Value = "Count";
sheet.Cells["B2"].Value = 1;
sheet.Cells["B3"].Value = 2;
sheet.Cells["B4"].Value = 3;
sheet.Cells["B5"].Value = 4;
// Create pivot table
int index = sheet.PivotTables.Add("A1:B5", "C3", "PivotTable1");
PivotTable pivotTable = sheet.PivotTables[index];
// Add row field and data field
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Apply count filter
PivotField rowField = pivotTable.RowFields[0];
rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
// Get the count filter
PivotFilter filter = rowField.GetPivotFilterByType(PivotFilterType.Count);
// Output filter details
Console.WriteLine("Filter Type: " + filter.FilterType);
Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
Console.WriteLine("Auto Filter: " + filter.AutoFilter);
wb.Save("PivotFilterExample.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../../pivotfilter/)
* enum [PivotFilterType](../../pivotfiltertype/)
* class [PivotField](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
