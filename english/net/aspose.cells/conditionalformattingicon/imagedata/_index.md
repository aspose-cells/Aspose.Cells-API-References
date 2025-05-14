---
title: ConditionalFormattingIcon.ImageData
second_title: Aspose.Cells for .NET API Reference
description: ConditionalFormattingIcon property. Gets the icon set data
type: docs
url: /net/aspose.cells/conditionalformattingicon/imagedata/
---
## ConditionalFormattingIcon.ImageData property

Gets the icon set data.

```csharp
public byte[] ImageData { get; }
```

### Examples

```csharp
// Called: byte[] imageData = worksheet.Cells["D8"].GetConditionalFormattingResult().ConditionalFormattingIcon.ImageData;
public void ConditionalFormattingIcon_Property_ImageData()
{
    Workbook wb = new Workbook(Constants.sourcePath + "example.xlsx");
    Worksheet worksheet = wb.Worksheets[0];
    byte[] imageData = worksheet.Cells["D8"].GetConditionalFormattingResult().ConditionalFormattingIcon.ImageData;
    Assert.AreEqual(imageData != null && imageData.Length != 0,true);
    using (Image image = Image.FromStream(new MemoryStream(imageData)))
    {
        Assert.AreEqual(16, image.Width);
        Assert.AreEqual(16, image.Height);
    }
}
```

### See Also

* class [ConditionalFormattingIcon](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


