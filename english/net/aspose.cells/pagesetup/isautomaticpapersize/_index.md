---
title: PageSetup.IsAutomaticPaperSize
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Indicates whether the paper size is automatic
type: docs
url: /net/aspose.cells/pagesetup/isautomaticpapersize/
---
## PageSetup.IsAutomaticPaperSize property

Indicates whether the paper size is automatic.

```csharp
public bool IsAutomaticPaperSize { get; }
```

### Examples

```csharp
// Called: Assert.IsTrue(workbook.Worksheets[0].PageSetup.IsAutomaticPaperSize);
[Test]
        public void Property_IsAutomaticPaperSize()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CellsJava42770.xml&quot;);
            Assert.IsTrue(workbook.Worksheets[0].PageSetup.IsAutomaticPaperSize);
            Assert.AreEqual(PaperSizeType.PaperA4, workbook.Worksheets[0].PageSetup.PaperSize);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


