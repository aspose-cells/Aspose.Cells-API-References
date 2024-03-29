---
title: ImageType
second_title: Aspose.Cells för .NET API-referens
description: Hämtar bildens bildformat.
type: docs
weight: 60
url: /sv/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

Hämtar bildens bildformat.

```csharp
public ImageType ImageType { get; }
```

### Exempel

```csharp

[C#]
//Instantiering av ett arbetsboksobjekt
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//infoga första bilden
int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
//Hämta det infogade bildobjektet
Picture pic1 = worksheet.Pictures[imgIndex1];
if(pic1.ImageType == Aspose.Cells.Drawing.ImageType.Png)
{
    //Bildens typ är png.";
}
//infoga andra bilden
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
//Hämta det infogade bildobjektet
Picture pic2 = worksheet.Pictures[imgIndex2];
if(pic2.ImageType == Aspose.Cells.Drawing.ImageType.Jpeg)
{
    //Bildens typ är jpg.";
}
```

### Se även

* enum [ImageType](../../imagetype)
* class [Picture](../../picture)
* namnutrymme [Aspose.Cells.Drawing](../../picture)
* hopsättning [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
