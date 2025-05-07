---
title: MsoFormatPicture.Brightness
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Represents the brightness modification for the picture in unit of percentage
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/brightness/
---
## MsoFormatPicture.Brightness property

Represents the brightness modification for the picture in unit of percentage.

```csharp
public double Brightness { get; set; }
```

### Remarks

It is between -100% and 100%. It works same as Excel 2007 or above version.

### Examples

```csharp
// Called: Assert.AreEqual(0, ps.GetPicture(true, 2).FormatPicture.Brightness);
[Test]
        public void Property_Brightness()
        {
            Workbook workbook = new Workbook(Constants.sourcePath + "CELLSNET53788_2.xlsx");
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            Assert.AreEqual(0, ps.GetPicture(true, 2).FormatPicture.Brightness);
            workbook.Save(Constants.destPath + "CELLSNET53788_2.xlsx");
            workbook = new Workbook(Constants.destPath + "CELLSNET53788_2.xlsx");
            ps = workbook.Worksheets[0].PageSetup;
            Assert.AreEqual(0, ps.GetPicture(true, 2).FormatPicture.Brightness);
        }
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


