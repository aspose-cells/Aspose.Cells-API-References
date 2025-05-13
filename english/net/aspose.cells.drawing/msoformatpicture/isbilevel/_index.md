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
public void MsoFormatPicture_Property_IsBiLevel()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    wb.Save(Constants.destPath + "example.xlsx");
    wb = new Workbook(Constants.destPath + "example.xlsx");
    Picture pic = wb.Worksheets[0].PageSetup.GetPicture(true, 0);
    Assert.IsTrue(pic.FormatPicture.IsGray);
    Assert.IsTrue(pic.FormatPicture.IsBiLevel);
}
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


