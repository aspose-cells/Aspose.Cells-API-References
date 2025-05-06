---
title: PageSetup.IsHFAlignMargins
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Indicates whether header and footer margins are aligned with the page margins. If this property is true the left header and footer will be aligned with the left margin and the right header and footer will be aligned with the right margin. This option is enabled by default
type: docs
url: /net/aspose.cells/pagesetup/ishfalignmargins/
---
## PageSetup.IsHFAlignMargins property

Indicates whether header and footer margins are aligned with the page margins. If this property is true, the left header and footer will be aligned with the left margin, and the right header and footer will be aligned with the right margin. This option is enabled by default.

```csharp
public bool IsHFAlignMargins { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(false, workbook.Worksheets[0].PageSetup.IsHFAlignMargins);
[Test]
        public void Property_IsHFAlignMargins()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSNET-43423.xlsx&quot;);
            Assert.AreEqual(false, workbook.Worksheets[0].PageSetup.IsHFAlignMargins);
            workbook.Save(Constants.destPath + &quot;CELLSNET-43423.xlsx&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSNET-43423.xlsx&quot;);
            Assert.AreEqual(false, workbook.Worksheets[0].PageSetup.IsHFAlignMargins);
        }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


