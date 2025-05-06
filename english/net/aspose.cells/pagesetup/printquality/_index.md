---
title: PageSetup.PrintQuality
second_title: Aspose.Cells for .NET API Reference
description: PageSetup property. Represents the print quality
type: docs
url: /net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Represents the print quality.

```csharp
public int PrintQuality { get; set; }
```

### Examples

```csharp
// Called: Assert.AreEqual(workbook.Worksheets[1].PageSetup.PrintQuality, 144);
[Test]
        public void Property_PrintQuality()            
        {
            Workbook workbook = new Workbook(Constants.sourcePath + &quot;CELLSJAVA-40829.xls&quot;);
            for (int i = 0; i &lt; workbook.Worksheets.Count; i++)
            {
                workbook.Worksheets[i].PageSetup.PrintQuality = 144;
            }
            workbook.Save(Constants.destPath + &quot;CELLSJAVA40829.xls&quot;);
            workbook = new Workbook(Constants.destPath + &quot;CELLSJAVA40829.xls&quot;);
            Assert.AreEqual(workbook.Worksheets[1].PageSetup.PrintQuality, 144);
    }
```

### See Also

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


