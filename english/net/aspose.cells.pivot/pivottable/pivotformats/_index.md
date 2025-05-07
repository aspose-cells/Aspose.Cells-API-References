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
// Called: pt.PivotFormats.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.Automatic,  PivotTableSelectionType.DataAndLabel,false, false, s);
[Test]
        public void Property_PivotFormats()
        {

            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + "CELLSJAVA45351.xlsx");
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
            workbook.Save(Constants.PivotTableDestPath + "CELLSJAVA45351.xlsx");
            Assert.IsTrue(ManualFileUtil.ManualCheckStringInZip(Constants.PivotTableDestPath + "CELLSJAVA45351.xlsx", "xl/pivotTables/pivotTable1.xml", new string[] { "field=\"4\" defaultSubtotal=\"1\"" }, true));
        }
```

### See Also

* class [PivotTableFormatCollection](../../pivottableformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


