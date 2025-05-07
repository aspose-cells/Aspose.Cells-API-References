---
title: StyleFlag.LeftBorder
second_title: Aspose.Cells for .NET API Reference
description: StyleFlag property. Left border settings will be applied
type: docs
url: /net/aspose.cells/styleflag/leftborder/
---
## StyleFlag.LeftBorder property

Left border settings will be applied.

```csharp
public bool LeftBorder { get; set; }
```

### Examples

```csharp
// Called: styleFlag.LeftBorder = true;
[Test]
        public void Property_LeftBorder()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            Cell cell = worksheet.Cells[0, 0];
            cell.Value = "A1";
            Style style = cell.GetStyle();
            style.HorizontalAlignment = TextAlignmentType.Center;
            StyleFlag styleFlag = new StyleFlag();
            styleFlag.HorizontalAlignment = true;
            cell.SetStyle(style, styleFlag);

            // Draw bottom border to range A1:C1

            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:C1");
            style = workbook.CreateStyle();
            Border border = style.Borders[BorderType.BottomBorder];
            border.LineStyle = CellBorderType.Thick;
            border.Color = Color.Red;
            styleFlag = new StyleFlag();
            styleFlag.BottomBorder = true;
            range.ApplyStyle(style, styleFlag);

            // Draw the left border to range A1:A10
            range = worksheet.Cells.CreateRange("A1:A10");
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

* class [StyleFlag](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


