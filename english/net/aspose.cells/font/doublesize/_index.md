---
title: Font.DoubleSize
second_title: Aspose.Cells for .NET API Reference
description: Font property. Gets and sets the double size of the font
type: docs
url: /net/aspose.cells/font/doublesize/
---
## Font.DoubleSize property

Gets and sets the double size of the font.

```csharp
public double DoubleSize { get; set; }
```

### Examples

```csharp
// Called: style.Font.DoubleSize = 10.5;
[Test]
        public void Property_DoubleSize()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet1 = workbook.Worksheets[0];
            Cells cells = worksheet1.Cells;
            Aspose.Cells.Cell cell = cells["A1"];
            string val = "Less Fee Waivers & Net Expenses Footnote.";
            cell.HtmlString = val; // error 
            Style style = cell.GetStyle();
            style.Font.DoubleSize = 10.5;
            cell.SetStyle(style);
            Assert.AreEqual(cell.HtmlString.IndexOf("10.5") != -1, true);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


