---
title: MsoFormatPicture.IsBiLevel
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Indicates whether this picture should display in twocolor black and white
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/isbilevel/
---
## MsoFormatPicture.IsBiLevel property

Indicates whether this picture should display in two-color black and white.

```csharp
public bool IsBiLevel { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(pic.FormatPicture.IsBiLevel);
[Test]
        public void Property_IsBiLevel()
        {
            Workbook wb = new Workbook(Constants.sourcePath + &quot;CELLSNET53287.xlsx&quot;);
            wb.Save(Constants.destPath + &quot;CELLSNET53287.xlsx&quot;);
            wb = new Workbook(Constants.destPath + &quot;CELLSNET53287.xlsx&quot;);
            Picture pic = wb.Worksheets[0].PageSetup.GetPicture(true, 0);
            Assert.IsTrue(pic.FormatPicture.IsGray);
            Assert.IsTrue(pic.FormatPicture.IsBiLevel);
        }
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


