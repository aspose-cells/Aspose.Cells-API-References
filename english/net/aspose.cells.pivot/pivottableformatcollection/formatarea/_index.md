---
title: PivotTableFormatCollection.FormatArea
second_title: Aspose.Cells for .NET API Reference
description: PivotTableFormatCollection method. Formats selected area
type: docs
url: /net/aspose.cells.pivot/pivottableformatcollection/formatarea/
---
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
// Called: pt.PivotFormats.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.Automatic,  PivotTableSelectionType.DataAndLabel,false, false, s);
public void PivotTableFormatCollection_Method_FormatArea()
{

    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
    PivotTable pt = workbook.Worksheets["PIVOT_VBA_SUBTOTALS"].PivotTables[0];
    //Style s = pivotArea.GetStyle(); //pointer to the style of the area and only add borders
    Style s = workbook.CreateStyle(); //instead of creating a new style
    s.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Red);
    s.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Red);
    s.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Red);
    s.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Red);
    s.Pattern = BackgroundType.Solid;
    s.ForegroundColor = Color.Red;
    s.BackgroundColor = Color.Red;

    pt.PivotFormats.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.Automatic,  PivotTableSelectionType.DataAndLabel,false, false, s);
    pt.RefreshDataOnOpeningFile = true;
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
    Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + "example.xlsx", "xl/pivotTables/pivotTable1.xml", new string[] { "field=\"4\" defaultSubtotal=\"1\"" }, true));
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


