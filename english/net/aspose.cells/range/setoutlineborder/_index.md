---
title: Range.SetOutlineBorder
second_title: Aspose.Cells for .NET API Reference
description: Range method. Sets outline border around a range of cells
type: docs
url: /net/aspose.cells/range/setoutlineborder/
---
## SetOutlineBorder(BorderType, CellBorderType, CellsColor) {#setoutlineborder}

Sets outline border around a range of cells.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, 
    CellsColor borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Border edge. |
| borderStyle | CellBorderType | Border style. |
| borderColor | CellsColor | Border color. |

### Examples

```csharp
// Called: range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);
[Test]
        public void Method_CellsColor_()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            CellsColor color = workbook.CreateCellsColor();
            color.ThemeColor = new ThemeColor(ThemeColorType.Accent2, 0);


            Color resColor = color.Color;
            Aspose.Cells.Range range = cells.CreateRange("A2:B3");
            range.SetOutlineBorder(BorderType.RightBorder, CellBorderType.Thin, color);
            Style style = range[0, 1].GetStyle();

            Assert.IsTrue(Util.CompareColor(resColor, style.Borders[BorderType.RightBorder].Color));


            range = cells.CreateRange("C6:F10");
            range.SetOutlineBorders(CellBorderType.Thin, color);
            style = range[0, 1].GetStyle();

            Console.WriteLine(style.Borders[BorderType.TopBorder].Color);
            workbook.Save(Constants.destPath + "CELLSNET51910.xlsx");
        }
```

### See Also

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorder(BorderType, CellBorderType, Color) {#setoutlineborder_1}

Sets outline border around a range of cells.

```csharp
public void SetOutlineBorder(BorderType borderEdge, CellBorderType borderStyle, Color borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderEdge | BorderType | Border edge. |
| borderStyle | CellBorderType | Border style. |
| borderColor | Color | Border color. |

### Examples

```csharp
// Called: row.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);
[Test]
        public void Method_Color_()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CellsNet47816.xlsx");
            var ws = workbook.Worksheets[0];
            var row = ws.Cells.CreateRange("21:21");
            Assert.AreEqual(44,ws.Cells.MaxColumn); // print 44
            row.SetOutlineBorder(BorderType.LeftBorder, CellBorderType.Double, Color.Black);
            row.SetOutlineBorder(BorderType.BottomBorder, CellBorderType.Double, Color.Black);
            Assert.AreEqual(44, ws.Cells.MaxColumn); // print 16383
            workbook.Save(Constants.destPath + "CellsNet47816.xlsx");
        }
```

### See Also

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


