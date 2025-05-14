---
title: MsoFormatPicture.Contrast
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Represents the contrast modification for the picture.in unit of percentage
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/contrast/
---
## MsoFormatPicture.Contrast property

Represents the contrast modification for the picture.in unit of percentage.

```csharp
public double Contrast { get; set; }
```

### Remarks

It is between -100% and 100%. It works same as Excel 2007 or above version.

### Examples

```csharp
// Called: Assert.AreEqual(87, Math.Round(picture.FormatPicture.Contrast));
public void MsoFormatPicture_Property_Contrast()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    wb.Combine(new Workbook(Constants.sourcePath + "example.xlsx"));
    wb.Combine(new Workbook(Constants.sourcePath + "example.xlsx"));
    Picture picture = wb.Worksheets[0].PageSetup.GetPicture(true, 1);
    Assert.AreEqual(85,picture.FormatPicture.Brightness);
    Assert.AreEqual(15, Math.Round(picture.FormatPicture.Contrast));
    picture = wb.Worksheets[1].PageSetup.GetPicture(true, 1);
    Assert.AreEqual(85, picture.FormatPicture.Brightness);
    Assert.AreEqual(15,Math.Round( picture.FormatPicture.Contrast));
    picture = wb.Worksheets[2].PageSetup.GetPicture(true, 1);
    Assert.AreEqual(85, picture.FormatPicture.Brightness);
    Assert.AreEqual(87, Math.Round(picture.FormatPicture.Contrast));

    wb = Util.ReSave(wb, SaveFormat.Xlsx);
    picture = wb.Worksheets[0].PageSetup.GetPicture(true, 1);
    Assert.AreEqual(85, picture.FormatPicture.Brightness);
    Assert.AreEqual(15, Math.Round(picture.FormatPicture.Contrast));
    picture = wb.Worksheets[1].PageSetup.GetPicture(true, 1);
    Assert.AreEqual(85, picture.FormatPicture.Brightness);
    Assert.AreEqual(15, Math.Round(picture.FormatPicture.Contrast));
    picture = wb.Worksheets[2].PageSetup.GetPicture(true, 1);
    Assert.AreEqual(85, picture.FormatPicture.Brightness);
    Assert.AreEqual(87, Math.Round(picture.FormatPicture.Contrast));
}
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


