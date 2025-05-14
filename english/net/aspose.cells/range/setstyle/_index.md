---
title: Range.SetStyle
second_title: Aspose.Cells for .NET API Reference
description: Range method. Apply the cell style
type: docs
url: /net/aspose.cells/range/setstyle/
---
## SetStyle(Style, bool) {#setstyle_1}

Apply the cell style.

```csharp
public void SetStyle(Style style, bool explicitFlag)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The cell style. |
| explicitFlag | Boolean | True, only overwriting formatting which is explicitly set. |

### Examples

```csharp
// Called: wb.Worksheets[0].Cells.CreateRange(0, 1, false).SetStyle(style, true);
public void Range_Method_SetStyle()
{
    Workbook wb = new Workbook();
    Style style = new CellsFactory().CreateStyle();
    style.Pattern = BackgroundType.Solid;
    style.ForegroundColor = Color.Red;
    wb.Worksheets[0].Cells.CreateRange(0, 1, false).SetStyle(style, true);
   Assert.IsTrue( wb.Worksheets[0].Cells.Rows[0].GetCellOrNull(3) == null);
    wb.Save(Constants.destPath + "example.xlsx");
}
```

### See Also

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetStyle(Style) {#setstyle}

Sets the style of the range.

```csharp
public void SetStyle(Style style)
```

| Parameter | Type | Description |
| --- | --- | --- |
| style | Style | The Style object. |

### Examples

```csharp
// Called: workbook.Worksheets[sheetIndex].Cells.CreateRange(startingCell, endingCell).SetStyle(style);
public static void Range_Method_SetStyle(Workbook workbook, int sheetIndex, string startingCell, string endingCell, string name, int size, bool isBold, bool isItalics, FontUnderlineType underline, Color color, bool isWrap)
        {
            BaseCellFontFormat(workbook, sheetIndex, startingCell, name, size, isBold, isItalics, underline, color, isWrap);
            Style style = workbook.Worksheets[sheetIndex].Cells[startingCell].GetStyle();
            workbook.Worksheets[sheetIndex].Cells.CreateRange(startingCell, endingCell).SetStyle(style);
        }
```

### See Also

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


