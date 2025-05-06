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
// Called: pt.PivotFormats.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.LabelOnly, false, false, s);
[Test]
        public void Property_PivotFormats()
        {
            // Now let&apos;s try with a copied workbook
            Workbook workbook = new Workbook(Constants.PivotTableSourcePath + &quot;CellsJava45283.xlsx&quot;);
            PivotTable pt = workbook.Worksheets[&quot;PIVOT&quot;].PivotTables[0];
            pt.RefreshDataOnOpeningFile = true;
            //Style s = pivotArea.GetStyle(); //pointer to the style of the area and only add borders
            Style s = workbook.CreateStyle(); //instead of creating a new style
            s.SetBorder(BorderType.LeftBorder, CellBorderType.Thin, Color.Black);
            s.SetBorder(BorderType.RightBorder, CellBorderType.Thin, Color.Black);
            s.SetBorder(BorderType.TopBorder, CellBorderType.Thin, Color.Black);
            s.SetBorder(BorderType.BottomBorder, CellBorderType.Thin, Color.Black);
            s.Pattern = (BackgroundType.Solid);
            s.BackgroundColor = (Color.Yellow);


            pt.PivotFormats.FormatArea(PivotFieldType.Row, 0, PivotFieldSubtotalType.None, PivotTableSelectionType.LabelOnly, false, false, s);

            workbook.Save(Constants.PivotTableDestPath + &quot;CellsJava45283.xlsx&quot;);
        }
```

### See Also

* class [PivotTableFormatCollection](../../pivottableformatcollection/)
* class [PivotTable](../)
* namespace [Aspose.Cells.Pivot](../../../aspose.cells.pivot/)
* assembly [Aspose.Cells](../../../)


