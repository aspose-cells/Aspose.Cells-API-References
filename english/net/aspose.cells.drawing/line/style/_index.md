---
title: Line.Style
second_title: Aspose.Cells for .NET API Reference
description: Line property. Represents the style of the line
type: docs
url: /net/aspose.cells.drawing/line/style/
---
## Line.Style property

Represents the style of the line.

```csharp
public LineType Style { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(charts[0].Title.Border.Style, LineType.MediumGray);
[Test]
        public void Property_Style()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "testLineStyle.xls");
            ChartCollection charts = workbook.Worksheets[0].Charts;
            Assert.AreEqual(charts[0].Title.Border.Style, LineType.MediumGray);
            Assert.AreEqual(charts[1].Title.Border.Style, LineType.DarkGray);
        }
```

### See Also

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


