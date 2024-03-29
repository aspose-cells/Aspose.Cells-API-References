---
title: Picture.ImageType
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets the image format of the picture
type: docs
url: /net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

Gets the image format of the picture.

```csharp
public ImageType ImageType { get; }
```

### Examples

```csharp

[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//insert first picture
int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
//Get the inserted picture object
Picture pic1 = worksheet.Pictures[imgIndex1];
if(pic1.ImageType == Aspose.Cells.Drawing.ImageType.Png)
{
    //The picture's type is png.";
}
//insert second picture
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
//Get the inserted picture object
Picture pic2 = worksheet.Pictures[imgIndex2];
if(pic2.ImageType == Aspose.Cells.Drawing.ImageType.Jpeg)
{
    //The picture's type is jpg.";
}
```

### See Also

* enum [ImageType](../../imagetype/)
* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


