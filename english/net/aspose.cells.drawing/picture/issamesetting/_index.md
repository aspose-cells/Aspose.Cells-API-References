---
title: Picture.IsSameSetting
second_title: Aspose.Cells for .NET API Reference
description: Picture method. Returns whether the shape is same
type: docs
url: /net/aspose.cells.drawing/picture/issamesetting/
---
## Picture.IsSameSetting method

Returns whether the shape is same.

```csharp
public override bool IsSameSetting(object obj)
```

| Parameter | Type | Description |
| --- | --- | --- |
| obj | Object |  |

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
//insert second picture
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
//Get the inserted picture object
Picture pic2 = worksheet.Pictures[imgIndex2];
if(pic1.IsSameSetting(pic1))
{
    //two image objects are the same.
}

if(!pic1.IsSameSetting(pic2))
{
    //two image objects are not the same.
}
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


