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
// Called: Assert.AreEqual(12.75, workbook.Worksheets[0].Cells.StandardHeight);
[Test]
        public void Property_StandardHeight()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsNet46198.xlsx&quot;);
            Assert.AreEqual(12.75, workbook.Worksheets[0].Cells.StandardHeight);
            workbook.Save(Constants.destPath + &quot;CellsNet46198.xlsx&quot;);
        }
```

### See Also

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


