---
title: Cell.GetStyle
second_title: Aspose.Cells for .NET API Reference
description: Cell method. Gets the cell style
type: docs
url: /net/aspose.cells/cell/getstyle/
---
## GetStyle() {#getstyle}

Gets the cell style.

```csharp
public Style GetStyle()
```

### Return Value

Style object.

### Remarks

To change the style of the cell, please call Cell.SetStyle() method after modifying the returned style object. This method is same with `GetStyle` with true value for the parameter.

### Examples

```csharp
// Called: checkColumnStyle(cells[65535, 5].GetStyle());
private void Method_GetStyle(Workbook workbook)
        {
            Cells cells = workbook.Worksheets[0].Cells;
            checkStyle(cells[3, 2].GetStyle());
            checkStyle(cells[3, 3].GetStyle());
            checkStyle(cells[4, 2].GetStyle());
            checkStyle(cells[4, 3].GetStyle());
            checkStyle(cells[5, 4].GetStyle());
            checkStyle(cells[5, 5].GetStyle());
            checkRowStyle(cells.Rows[7].GetStyle());
            for (int row = 0; row &lt;= 4; row++)
            {
                checkColumnStyle(cells[row, 5].GetStyle());
            }
            checkColumnStyle(cells[5, 7].GetStyle());
            checkColumnStyle(cells[6, 7].GetStyle());
            checkColumnStyle(cells[8, 5].GetStyle());
            checkColumnStyle(cells[9, 5].GetStyle());
            checkColumnStyle(cells[86, 5].GetStyle());
            checkColumnStyle(cells[219, 5].GetStyle());
            checkColumnStyle(cells[1698, 5].GetStyle());
            checkColumnStyle(cells[5002, 5].GetStyle());
            checkColumnStyle(cells[10982, 5].GetStyle());
            checkColumnStyle(cells[30090, 5].GetStyle());
            checkColumnStyle(cells[65534, 5].GetStyle());
            checkColumnStyle(cells[65535, 5].GetStyle());
        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)

---

## GetStyle(bool) {#getstyle_1}

If checkBorders is true, check whether other cells' borders will effect the style of this cell.

```csharp
public Style GetStyle(bool checkBorders)
```

| Parameter | Type | Description |
| --- | --- | --- |
| checkBorders | Boolean | Check other cells' borders |

### Return Value

Style object.

### Examples

```csharp
// Called: Style style = cell.GetStyle(false);
[Test]
        public void Method_Boolean_()
        {
            Workbook wb = new Workbook();
            Cell cell = wb.Worksheets[0].Cells[0, 0];
            cell.PutValue(45734);
            Style style = cell.GetStyle(false);
            style.Custom = &quot;[DBNum1]上午/下午h\&quot;时\&quot;mm\&quot;分\&quot;&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;上午12时00分&quot;, cell.StringValue, &quot;h&quot;);
            style.Custom = &quot;[DBNum1]上午/下午hh\&quot;时\&quot;mm\&quot;分\&quot;&quot;;
            cell.SetStyle(style);
            Assert.AreEqual(&quot;上午12时00分&quot;, cell.StringValue, &quot;hh&quot;);
        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


