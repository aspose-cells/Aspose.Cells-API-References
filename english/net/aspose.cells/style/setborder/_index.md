---
title: Style.SetBorder
second_title: Aspose.Cells for .NET API Reference
description: Style method. Sets the borders of the style
type: docs
url: /net/aspose.cells/style/setborder/
---
## SetBorder(BorderType, CellBorderType, Color) {#setborder_1}

Sets the borders of the style.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, Color borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | BorderType | The border(s) to be set, can be combination of [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | The style of the border. |
| borderColor | Color | The color of the border. |

### Return Value

Whether current border settings have been changed.

### Examples

```csharp
// Called: style.SetBorder(BorderType.LeftBorder, pHigh, Color.Red);
private void Method_Color_(CellBorderType pLow, CellBorderType pMid, CellBorderType pHigh)
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;
            cells.Columns[2].IsHidden = true;
            Style style = wb.CreateStyle();
            int row = 0;
            style.SetBorder(BorderType.RightBorder, pLow, Color.Red);
            cells[row, 1].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pLow, Color.Red);
            style.SetBorder(BorderType.RightBorder, pHigh, Color.Red);
            cells[row, 2].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pHigh, Color.Red);
            cells[row, 3].SetStyle(style);
            Assert.AreEqual(pLow, cells[row, 1].GetStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.Style.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.Style.LeftBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.DisplayStyle.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.DisplayStyle.LeftBorder&quot;);
            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.RightBorder, pHigh, Color.Red);
            cells[row, 1].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pHigh, Color.Red);
            style.SetBorder(BorderType.RightBorder, pLow, Color.Red);
            cells[row, 2].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pLow, Color.Red);
            cells[row, 3].SetStyle(style);
            Assert.AreEqual(pHigh, cells[row, 1].GetStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.Style.RightBorder&quot;);
            Assert.AreEqual(pLow, cells[row, 3].GetStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.Style.LeftBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.DisplayStyle.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.DisplayStyle.LeftBorder&quot;);

            row++;
            style.SetBorder(BorderType.RightBorder, pLow, Color.Red);
            cells[row, 1].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pMid, Color.Red);
            style.SetBorder(BorderType.RightBorder, pHigh, Color.Red);
            cells[row, 2].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pMid, Color.Red);
            cells[row, 3].SetStyle(style);
            Assert.AreEqual(pMid, cells[row, 1].GetStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.Style.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.Style.LeftBorder&quot;);
            Assert.AreEqual(pMid, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.DisplayStyle.RightBorder&quot;);
            Assert.AreEqual(pMid, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.DisplayStyle.LeftBorder&quot;);
            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.RightBorder, pHigh, Color.Red);
            cells[row, 1].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pMid, Color.Red);
            style.SetBorder(BorderType.RightBorder, pMid, Color.Red);
            cells[row, 2].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pLow, Color.Red);
            cells[row, 3].SetStyle(style);
            Assert.AreEqual(pHigh, cells[row, 1].GetStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.Style.RightBorder&quot;);
            Assert.AreEqual(pMid, cells[row, 3].GetStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.Style.LeftBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.DisplayStyle.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.DisplayStyle.LeftBorder&quot;);

            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pLow, Color.Red);
            style.SetBorder(BorderType.RightBorder, pHigh, Color.Red);
            cells[row, 2].SetStyle(style);
            Assert.AreEqual(CellBorderType.None, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.RightBorder&quot;);
            Assert.AreEqual(CellBorderType.None, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.LeftBorder&quot;);
            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pHigh, Color.Red);
            style.SetBorder(BorderType.RightBorder, pLow, Color.Red);
            cells[row, 2].SetStyle(style);
            Assert.AreEqual(CellBorderType.None, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.RightBorder&quot;);
            Assert.AreEqual(CellBorderType.None, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.LeftBorder&quot;);

            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.RightBorder, pLow, Color.Red);
            cells[row, 1].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.RightBorder, pHigh, Color.Red);
            cells[row, 2].SetStyle(style);
            Assert.AreEqual(pLow, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.RightBorder&quot;);
            Assert.AreEqual(pLow, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.LeftBorder&quot;);
            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.RightBorder, pHigh, Color.Red);
            cells[row, 1].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.RightBorder, pLow, Color.Red);
            cells[row, 2].SetStyle(style);
            Assert.AreEqual(pHigh, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.LeftBorder&quot;);

            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pLow, Color.Red);
            cells[row, 2].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pHigh, Color.Red);
            cells[row, 3].SetStyle(style);
            Assert.AreEqual(pHigh, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.LeftBorder&quot;);
            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pHigh, Color.Red);
            cells[row, 2].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pLow, Color.Red);
            cells[row, 3].SetStyle(style);
            Assert.AreEqual(pLow, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.RightBorder&quot;);
            Assert.AreEqual(pLow, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.LeftBorder&quot;);

            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.RightBorder, pLow, Color.Red);
            cells[row, 1].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pHigh, Color.Red);
            cells[row, 3].SetStyle(style);
            Assert.AreEqual(pHigh, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.LeftBorder&quot;);
            row++;
            style = wb.CreateStyle();
            style.SetBorder(BorderType.RightBorder, pHigh, Color.Red);
            cells[row, 1].SetStyle(style);
            style = wb.CreateStyle();
            style.SetBorder(BorderType.LeftBorder, pLow, Color.Red);
            cells[row, 3].SetStyle(style);
            Assert.AreEqual(pHigh, cells[row, 1].GetDisplayStyle().Borders[BorderType.RightBorder].LineStyle,
                &quot;B&quot; + (row + 1) + &quot;.RightBorder&quot;);
            Assert.AreEqual(pHigh, cells[row, 3].GetDisplayStyle().Borders[BorderType.LeftBorder].LineStyle,
                &quot;D&quot; + (row + 1) + &quot;.LeftBorder&quot;);
        }
```

### See Also

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## SetBorder(BorderType, CellBorderType, CellsColor) {#setborder}

Sets the borders of the style.

```csharp
public bool SetBorder(BorderType borderType, CellBorderType borderStyle, CellsColor borderColor)
```

| Parameter | Type | Description |
| --- | --- | --- |
| borderType | BorderType | The border(s) to be set, can be combination of [`BorderType`](../../bordertype/). |
| borderStyle | CellBorderType | The style of the border. |
| borderColor | CellsColor | The color of the border. |

### Return Value

Whether current border settings have been changed.

### See Also

* enum [BorderType](../../bordertype/)
* enum [CellBorderType](../../cellbordertype/)
* class [CellsColor](../../cellscolor/)
* class [Style](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


