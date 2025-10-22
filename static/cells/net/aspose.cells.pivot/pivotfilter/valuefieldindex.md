##PivotFilter.ValueFieldIndex
PivotFilter property. Gets the index of value field in the value region
## PivotFilter.ValueFieldIndex property
Gets the index of value field in the value region.
```csharp
public int ValueFieldIndex { get; set; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterPropertyValueFieldIndexDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["B1"].Value = "Quantity";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["B2"].Value = 10;
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["B3"].Value = 5;
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B4"].Value = 7;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "D1", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
// Add fields to pivot table
pivotTable.AddFieldToArea(PivotFieldType.Row, 0); // Fruit
pivotTable.AddFieldToArea(PivotFieldType.Data, 1); // Quantity
// Add count filter to row field
PivotField rowField = pivotTable.RowFields[0];
rowField.FilterTop10(0, PivotFilterType.Count, true, 2);
// Get the filter and demonstrate ValueFieldIndex
PivotFilter filter = rowField.GetFilters()[0];
Console.WriteLine("Filter Type: " + filter.FilterType);
Console.WriteLine("Value Field Index: " + filter.ValueFieldIndex);
// Save the workbook
workbook.Save("PivotFilterValueFieldIndexDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
