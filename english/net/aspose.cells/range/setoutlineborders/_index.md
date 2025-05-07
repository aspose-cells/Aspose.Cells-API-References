---
title: Range.SetOutlineBorders
second_title: Aspose.Cells for .NET API Reference
description: Range method. Sets the outline borders around a range of cells with same border style and color
type: docs
url: /net/aspose.cells/range/setoutlineborders/
---
## SetOutlineBorders(CellBorderType, CellsColor) {#setoutlineborders}

Sets the outline borders around a range of cells with same border style and color.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, CellsColor borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Border style. |
| borderColor | CellsColor | Border color. |

### Examples

```csharp
// Called: range.SetOutlineBorders(CellBorderType.Thin, color);
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

* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType, Color) {#setoutlineborders_1}

Sets the outline borders around a range of cells with same border style and color.

```csharp
public void SetOutlineBorders(CellBorderType borderStyle, Color borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | CellBorderType | Border style. |
| borderColor | Color | Border color. |

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetOutlineBorders(CellBorderType[], Color[]) {#setoutlineborders_2}

Sets out line borders around a range of cells.

```csharp
public void SetOutlineBorders(CellBorderType[] borderStyles, Color[] borderColors)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderStyles | CellBorderType[] | Border styles. |
| borderColors | Color[] | Border colors. |

### Remarks

Both the length of borderStyles and borderStyles must be 4. The order of borderStyles and borderStyles must be top,bottom,left,right

### See Also

* enum [CellBorderType](../../cellbordertype/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


