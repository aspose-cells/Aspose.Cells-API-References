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
// Called: Assert.AreEqual(30,ps.GetPicture(true, 0).FormatPicture.Brightness);
public void MsoFormatPicture_Property_Brightness()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    PageSetup ps = workbook.Worksheets[0].PageSetup;
    Assert.AreEqual(30,ps.GetPicture(true, 0).FormatPicture.Brightness);
    // Console.WriteLine(ps.GetPicture(true, 1).FormatPicture.Brightness);
    Assert.AreEqual(100, ps.GetPicture(true, 2).FormatPicture.Brightness);
    Assert.AreEqual(80, ps.GetPicture(false, 1).FormatPicture.Brightness);
    Assert.AreEqual(50, ps.GetPicture(false, 2).FormatPicture.Brightness);
}
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


