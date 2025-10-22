##PivotTableFormatCollection.Item
PivotTableFormatCollection property. Gets the format by the index
## PivotTableFormatCollection indexer
Gets the format by the index.
```csharp
public PivotTableFormat this[int index] { get; }
```
| Parameter | Description |
| --- | --- |
| index | The index. |
### Examples
```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Pivot;
namespace AsposeCellsExamples
{
public class PivotTableFormatCollectionPropertyItemDemo
{
public static void Run()
{
// Create a workbook from source Excel file
Workbook workbook = new Workbook("example.xlsx");
// Refresh all pivot tables
workbook.Worksheets.RefreshAll();
Cells cells = workbook.Worksheets[0].Cells;
// Access the first pivot table
PivotTable pt = workbook.Worksheets[0].PivotTables[0];
// Demonstrate Item property by accessing the first PivotFormat
pt.PivotFormats[0].PivotArea.OnlyData = false;
workbook.Worksheets.RefreshAll();
// Change format settings using Item property
pt.PivotFormats[0].PivotArea.OnlyLabel = true;
workbook.Worksheets.RefreshAll();
// Save the modified workbook
workbook.Save("modified_example.xlsx");
}
}
}
```
### See Also
* class [PivotTableFormat](../../pivottableformat/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
