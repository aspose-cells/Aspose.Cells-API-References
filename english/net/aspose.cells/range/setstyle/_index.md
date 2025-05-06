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
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Style style = new CellsFactory().CreateStyle();
            style.Pattern = BackgroundType.Solid;
            style.ForegroundColor = Color.Red;
            wb.Worksheets[0].Cells.CreateRange(0, 1, false).SetStyle(style, true);
           Assert.IsTrue( wb.Worksheets[0].Cells.Rows[0].GetCellOrNull(3) == null);
            wb.Save(Constants.destPath + &quot;CELLSNET57109.xlsx&quot;);
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
// Called: workbook.Worksheets[sheetIndex].Cells.CreateRange(startingRow, startingColumn, rowCount, columnCount).SetStyle(style2);
public static void Method_Style_(Workbook workbook, int sheetIndex, int startingRow, int startingColumn, int rowCount, int columnCount, string name, int size, bool isBold, bool isItalics, FontUnderlineType underline, Color color, bool isWrap)
        {
            startingRow--;
            startingColumn--;
            Style style = workbook.CreateStyle();
            style.Font.Name = name;
            style.Font.Size = size;
            style.Font.IsBold = isBold;
            style.Font.IsItalic = isItalics;
            style.Font.Underline = underline;
            style.Font.Color = color;
            style.IsTextWrapped = isWrap;
            workbook.Worksheets[sheetIndex].Cells[startingRow, startingColumn].SetStyle(style);
            Style style2 = workbook.Worksheets[sheetIndex].Cells[startingRow, startingColumn].GetStyle();
            workbook.Worksheets[sheetIndex].Cells.CreateRange(startingRow, startingColumn, rowCount, columnCount).SetStyle(style2);
        }
```

### See Also

* class [Style](../../style/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


