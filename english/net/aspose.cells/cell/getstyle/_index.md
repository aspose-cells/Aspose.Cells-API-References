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
// Called: Style style = cells["B11"].GetStyle();
[Test]
        public void Method_GetStyle()
        {
            var wb = new Workbook(Constants.sourcePath + @"Numbers13\CELLSNET48344.numbers");
            Cells cells = wb.Worksheets[0].Cells;
            Style style = cells["B11"].GetStyle();

            Assert.AreEqual(BackgroundType.Solid, style.Pattern);
            AssertHelper.AreEqual(Color.Red, style.ForegroundColor);
            style = cells["E11"].GetStyle();
            Assert.AreEqual(BackgroundType.None, style.Pattern);
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
// Called: Assert.AreEqual(11.5, _cell.GetStyle(false).Font.DoubleSize);
[Test]
        public void Method_Boolean_()
        {
            var _book = new Workbook();
            var _sheet = _book.Worksheets[0];
            var _cell = _sheet.Cells[0, 0];
            _cell.HtmlString = "<font style=\"font-size:11.5pt\">Test string</font>";
            Assert.AreEqual(11.5, _cell.GetStyle(false).Font.DoubleSize);
            _book.Save(Constants.destPath + "CellsNet47658.xlsx");
        }
```

### See Also

* class [Style](../../style/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


