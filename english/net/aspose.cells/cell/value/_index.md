---
title: Cell.Value
second_title: Aspose.Cells for .NET API Reference
description: Cell property. Gets/sets the value contained in this cell
type: docs
url: /net/aspose.cells/cell/value/
---
## Cell.Value property

Gets/sets the value contained in this cell.

```csharp
public object Value { get; set; }
```

### Remarks

Possible type:

null,

Boolean,

DateTime,

Double,

Integer

String.

For int value, it may be returned as an Integer object or a Double object. And there is no guarantee that the returned value will be kept as the same type of object always.

### Examples

```csharp
// Called: cell.Value = &amp;quot;A1&amp;quot;;
[Test]
        public void Property_Value()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cell cell = worksheet.Cells[0, 0];
            cell.Value = &quot;A1&quot;;
            Style style = cell.GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            cell.SetStyle(style, styleFlag);

            // Draw bottom border to range A1:C1

            Aspose.Cells.Range range = worksheet.Cells.CreateRange(&quot;A1:C1&quot;);
            style = workbook.CreateStyle();
            Border border = style.Borders[BorderType.BottomBorder];
            border.LineStyle = CellBorderType.Thick;
            border.Color = Color.Red;
            styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;
            range.ApplyStyle(style, styleFlag);

            // Draw the left border to range A1:A10
            range = worksheet.Cells.CreateRange(&quot;A1:A10&quot;);
            style = workbook.CreateStyle();
            border = style.Borders[BorderType.LeftBorder];
            border.LineStyle = CellBorderType.Thick;
            border.Color = Color.Green;
            styleFlag = new StyleFlag();
            styleFlag.LeftBorder = true;
            range.ApplyStyle(style, styleFlag);
            cell = worksheet.Cells[0, 0];
            Assert.AreEqual(TextAlignmentType.Center, cell.GetStyle().HorizontalAlignment);
            Assert.AreEqual(CellBorderType.Thick, cell.GetStyle().Borders[BorderType.BottomBorder].LineStyle);
        }
```

### See Also

* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


