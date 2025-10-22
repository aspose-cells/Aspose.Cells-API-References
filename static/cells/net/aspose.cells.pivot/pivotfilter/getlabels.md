##PivotFilter.GetLabels
PivotFilter method. Gets labels of the caption filter
## PivotFilter.GetLabels method
Gets labels of the caption filter.
```csharp
public string[] GetLabels()
```
### Examples
```csharp
namespace AsposeCellsExamples
{
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System;
public class PivotFilterMethodGetLabelsDemo
{
public static void Run()
{
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
try
{
// Create valid pivot table structure
worksheet.Cells["A1"].Value = "Category";
worksheet.Cells["A2"].Value = "A";
worksheet.Cells["A3"].Value = "B";
worksheet.Cells["A4"].Value = "A";
// Create pivot table with correct parameters
int pivotIndex = worksheet.PivotTables.Add("A1:A4", "C3", "PivotTable1");
PivotTable pivotTable = worksheet.PivotTables[pivotIndex];
// Create pivot filter with valid parameters
int filterIndex = pivotTable.PivotFilters.Add(0, PivotFilterType.CaptionEqual);
PivotFilter pivotFilter = pivotTable.PivotFilters[filterIndex];
// Configure filter properties
pivotFilter.Name = "SampleFilter";
pivotFilter.EvaluationOrder = 1;
// Execute GetLabels method
string[] labels = pivotFilter.GetLabels();
Console.WriteLine($"Retrieved {labels?.Length ?? 0} labels:");
if (labels != null)
{
foreach (string label in labels)
{
Console.WriteLine($"- {label}");
}
}
workbook.Save("GetLabelsDemo.xlsx");
}
catch (Exception ex)
{
Console.WriteLine($"Error calling GetLabels: {ex.Message}");
}
}
}
}
```
### See Also
* class [PivotFilter](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
