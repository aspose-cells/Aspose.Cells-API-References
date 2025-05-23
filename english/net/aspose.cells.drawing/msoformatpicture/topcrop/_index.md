---
title: MsoFormatPicture.TopCrop
second_title: Aspose.Cells for .NET API Reference
description: MsoFormatPicture property. Represents the location of the top of the crop rectangle expressed expressed as a ratio of the images height
type: docs
url: /net/aspose.cells.drawing/msoformatpicture/topcrop/
---
## MsoFormatPicture.TopCrop property

Represents the location of the top of the crop rectangle expressed, expressed as a ratio of the image's height.

```csharp
public double TopCrop { get; set; }
```

### Examples

```csharp
// Called: Assert.IsTrue(pic.FormatPicture.TopCrop < -5);
public void MsoFormatPicture_Property_TopCrop()
{
    Workbook workbook = new Workbook(Constants.sourcePath + "example.xlsx");
    PageSetup ps = workbook.Worksheets[0].PageSetup;
    Picture pic = ps.GetPicture(true, 1);
    Assert.IsTrue(pic.FormatPicture.TopCrop < -5);
}
```

### See Also

* class [MsoFormatPicture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


