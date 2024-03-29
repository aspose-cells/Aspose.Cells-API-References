---
title: Picture.Data
second_title: Aspose.Cells for .NET API Reference
description: Picture property. Gets the data of the picture
type: docs
url: /net/aspose.cells.drawing/picture/data/
---
## Picture.Data property

Gets the data of the picture.

```csharp
public byte[] Data { get; set; }
```

### Examples

```csharp

[C#]
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//insert first picture
int imgIndex1 = worksheet.Pictures.Add(1, 1, "example1.png");
//Get the inserted picture object
Picture pic1 = worksheet.Pictures[imgIndex1];
//insert second picture
int imgIndex2 = worksheet.Pictures.Add(1, 9, "example2.jpeg");
//Get the inserted picture object
Picture pic2 = worksheet.Pictures[imgIndex2];
//Assign the byte data of the first image to the second image
pic2.Data = pic1.Data;
//Save the excel file.
workbook.Save("result.xlsx");
```

### See Also

* class [Picture](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


