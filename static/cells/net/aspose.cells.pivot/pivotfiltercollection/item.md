##PivotFilterCollection.Item
PivotFilterCollection property. Gets the pivotfilter object at the specific index
## PivotFilterCollection indexer
Gets the pivotfilter object at the specific index.
```csharp
public PivotFilter this[int index] { get; }
```
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotFilterCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook with sample data
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
// Add sample data for pivot table
worksheet.Cells["A1"].Value = "Fruit";
worksheet.Cells["A2"].Value = "Apple";
worksheet.Cells["A3"].Value = "Orange";
worksheet.Cells["A4"].Value = "Banana";
worksheet.Cells["B1"].Value = "Sales";
worksheet.Cells["B2"].Value = 100;
worksheet.Cells["B3"].Value = 200;
worksheet.Cells["B4"].Value = 150;
// Create pivot table
int index = worksheet.PivotTables.Add("A1:B4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[index];
pivotTable.AddFieldToArea(PivotFieldType.Row, 0);
pivotTable.AddFieldToArea(PivotFieldType.Data, 1);
// Add pivot filter using PivotFilterCollection.Add method
pivotTable.PivotFilters.Add(0, PivotFilterType.Count);
PivotFilter filter = pivotTable.PivotFilters[0]; // Using Item property via index
filter.Name = "SampleFilter";
filter.Value1 = "100";
// Access filter using Item property and display information
Console.WriteLine("Filter Name: " + pivotTable.PivotFilters[0].Name);
Console.WriteLine("Filter Value1: " + pivotTable.PivotFilters[0].Value1);
Console.WriteLine("Filter Type: " + pivotTable.PivotFilters[0].FilterType);
// Save the workbook
workbook.Save("PivotFilterDemo.xlsx");
}
}
}
```
### See Also
* class [PivotFilter](../../pivotfilter/)
* class [PivotFilterCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
