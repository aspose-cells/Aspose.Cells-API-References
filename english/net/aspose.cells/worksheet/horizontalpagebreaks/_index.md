---
title: Worksheet.HorizontalPageBreaks
second_title: Aspose.Cells for .NET API Reference
description: Worksheet property. Gets the HorizontalPageBreakCollection collection
type: docs
url: /net/aspose.cells/worksheet/horizontalpagebreaks/
---
## Worksheet.HorizontalPageBreaks property

Gets the [`HorizontalPageBreakCollection`](../../horizontalpagebreakcollection/) collection.

```csharp
public HorizontalPageBreakCollection HorizontalPageBreaks { get; }
```

### Examples

```csharp
// Called: breaks = workbook.Worksheets[0].HorizontalPageBreaks;
[Test]
        public void Property_HorizontalPageBreaks()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET48675.xlsx&quot;);
            HorizontalPageBreakCollection breaks = workbook.Worksheets[0].HorizontalPageBreaks;
            Assert.AreEqual(2, breaks.Count);
            Assert.AreEqual(6, breaks[0].Row);
            Assert.AreEqual(12, breaks[1].Row);
            workbook.Save(Constants.destPath + &quot;CELLSNET48675.ods&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET48675.ods&quot;);
             breaks = workbook.Worksheets[0].HorizontalPageBreaks;
            Assert.AreEqual(2, breaks.Count);
            Assert.AreEqual(6, breaks[0].Row);
            Assert.AreEqual(12, breaks[1].Row);
            workbook.Save(Constants.destPath + &quot;CELLSNET48675.xlsx&quot;);
        }
```

### See Also

* class [HorizontalPageBreakCollection](../../horizontalpagebreakcollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


