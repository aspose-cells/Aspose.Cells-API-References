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
// Called: pt.PivotFormats.FormatArea(PivotFieldType.Data, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.DataAndLabel, false, false, s);
[Test]
        public void Method_Style_()
        {
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSJAVA45189.xlsx");
            PivotTable pt = workbook.Worksheets["PIVOT"].PivotTables[0];
            Style s = workbook.CreateStyle(); //instead of creating a new style
            s.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            s.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            s.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            s.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            s.Pattern = BackgroundType.Solid;
            // s.ForegroundColor = Color.Red;
            s.BackgroundColor = Color.Red;

            pt.PivotFormats.FormatArea(PivotFieldType.Data, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.DataAndLabel, false, false, s);

            pt.RefreshDataOnOpeningFile = true;
            workbook.Save(Constants.PivotTableDestPath + "CELLSJAVA45189.xlsx");
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


