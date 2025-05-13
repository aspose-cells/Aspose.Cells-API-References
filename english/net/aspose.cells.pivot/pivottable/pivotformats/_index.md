---
title: PivotTable.PivotFormats
second_title: Aspose.Cells for .NET API Reference
description: PivotTable property. Gets the collection of formats applied to PivotTable
type: docs
url: /net/aspose.cells.pivot/pivottable/pivotformats/
---
## PivotTable.PivotFormats property

Gets the collection of formats applied to PivotTable.

```csharp
public PivotTableFormatCollection PivotFormats { get; }
```

### Examples

```csharp
// Called: pt.PivotFormats.FormatArea(PivotFieldType.Data, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.DataAndLabel, false, false, s);
public void PivotTable_Property_PivotFormats()
{
    Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "example.xlsx");
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
    workbook.Save(Constants.PivotTableDestPath + "example.xlsx");
}
```

### See Also

* class [PivotTableFormatCollection](../../pivottableformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


