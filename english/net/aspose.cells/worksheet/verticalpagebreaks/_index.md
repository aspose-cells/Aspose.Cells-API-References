---
title: Worksheet.VerticalPageBreaks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the VerticalPageBreakCollection collection
type: docs
url: /net/aspose.cells/worksheet/verticalpagebreaks/
---
## Worksheet.VerticalPageBreaks property

Gets the [`VerticalPageBreakCollection`](../../verticalpagebreakcollection/) collection.

```csharp
public VerticalPageBreakCollection VerticalPageBreaks { get; }
```

### Examples

```csharp
// Called: Assert.AreEqual(1, workbook.Worksheets[0].VerticalPageBreaks.Count);
[Test]
        public void Property_VerticalPageBreaks()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET46640.xlsx");
            workbook.Save(Constants.destPath + "CELLSNET46640.ods");
            workbook = new Workbook(Constants.destPath + "CELLSNET46640.ods");
            Assert.AreEqual(1, workbook.Worksheets[0].HorizontalPageBreaks.Count);
            Assert.AreEqual(1, workbook.Worksheets[0].VerticalPageBreaks.Count);
            workbook.Save(Constants.destPath + "CELLSNET46640.xlsx");
        }
```

### See Also

* class [VerticalPageBreakCollection](../../verticalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


