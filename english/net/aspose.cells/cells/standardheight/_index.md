---
title: Cells.StandardHeight
second_title: Aspose.Cells for .NET API Reference
description: Cells property. Gets or sets the default row height in this worksheet in unit of points
type: docs
url: /net/aspose.cells/cells/standardheight/
---
## Cells.StandardHeight property

Gets or sets the default row height in this worksheet, in unit of points.

```csharp
public double StandardHeight { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(12.75, w1.Worksheets[0].Cells.StandardHeight);
[Test]
        public void Property_StandardHeight()
        {
            Workbook w1 = new Workbook();
           Assert.AreEqual(12.75,w1.Worksheets[0].Cells.StandardHeight);
            Style style = w1.Worksheets[0].Cells["A1"].GetStyle();
            style.IsTextWrapped = (true);
            w1.Worksheets[0].Cells["A1"].SetStyle(style);
            w1.Worksheets[0].Cells["A1"].Value = ("LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT");
            w1.Worksheets[0].Cells["A2"].Value = ("SOME OTHER LOOOOOOOOOOOOOOOOOONG TEEEEEEEEEEXT");
            w1.Worksheets[0].AutoFitRow(0);
            Assert.AreEqual(12.75, w1.Worksheets[0].Cells.StandardHeight);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


