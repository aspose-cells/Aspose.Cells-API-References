##PivotTableFormatCollection.FormatArea
PivotTableFormatCollection method. Formats selected area
## PivotTableFormatCollection.FormatArea method
Formats selected area.
```csharp
public PivotTableFormat FormatArea(PivotFieldType axisType, int fieldPosition,
PivotFieldSubtotalType subtotalType, PivotTableSelectionType selectionType, bool isGrandRow,
bool isGrandColumn, Style style)
```
| Parameter | Type | Description |
| --- | --- | --- |
| axisType | PivotFieldType | The region of the PivotTable to which this rule applies. |
| fieldPosition | Int32 | Position of the field within the axis to which this rule applies. |
| subtotalType | PivotFieldSubtotalType | The subtotal filter type of the pivot field |
| selectionType | PivotTableSelectionType | Indicates how to select data. |
| isGrandRow | Boolean | Indicates whether selecting grand total rows. |
| isGrandColumn | Boolean | Indicates whether selecting grand total columns. |
| style | Style | The style which appies to the area of the pivot table. |
### Examples
```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Pivot;
using System.Drawing;
namespace AsposeCellsExamples
{
public class PivotTableFormatCollectionMethodFormatAreaWithPivotFieldTypeInt32PivotFieldSDemo
{
public static void Run()
{
// Create a workbook from source file
Workbook workbook = new Workbook("example.xlsx");
// Access the pivot table
PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
// Create a style for formatting
Style style = workbook.CreateStyle();
style.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
style.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
style.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
style.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
style.Pattern = BackgroundType.Solid;
style.ForegroundColor = Color.LightGray;
style.BackgroundColor = Color.LightGray;
// Format the pivot table area
pt.PivotFormats.FormatArea(
PivotFieldType.Row,
0,
PivotFieldSubtotalType.Automatic,
PivotTableSelectionType.DataAndLabel,
false,
false,
style);
// Save the workbook
workbook.Save("output.xlsx");
}
}
}
```
### See Also
* class [PivotTableFormat](../../pivottableformat/)
* enum [PivotFieldType](../../pivotfieldtype/)
* enum [PivotFieldSubtotalType](../../pivotfieldsubtotaltype/)
* enum [PivotTableSelectionType](../../pivottableselectiontype/)
* class [Style](../../../aspose.cells/style/)
* class [PivotTableFormatCollection](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)
