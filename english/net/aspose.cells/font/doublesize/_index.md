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
// Called: Assert.AreEqual(workbook.Worksheets[0].Cells[&amp;quot;C4&amp;quot;].GetStyle().Font.DoubleSize, 16.5);
[Test]
        public void Property_DoubleSize()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet40407.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C4&quot;].GetStyle().Font.DoubleSize, 16.5);
            workbook.Save(Constants.destPath + &quot;CellsNet40407.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CellsNet40407.xlsx&quot;);
            Assert.AreEqual(workbook.Worksheets[0].Cells[&quot;C4&quot;].GetStyle().Font.DoubleSize, 16.5);
        }
```

### See Also

* class [Font](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


