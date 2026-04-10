---
title: Aspose::Cells::Drawing::Picture::GetBorderLineColor method
linktitle: GetBorderLineColor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetBorderLineColor method. Represents the Color of the border line of a picture in C++.'
type: docs
weight: 1100
url: /sv/cpp/aspose.cells.drawing/picture/getborderlinecolor/
---
## Picture::GetBorderLineColor method


Represents the [Color](../../../aspose.cells/color/) of the border line of a picture.

```cpp
Aspose::Cells::Color Aspose::Cells::Drawing::Picture::GetBorderLineColor()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instansierar ett Workbook‑objekt
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Lägger till en bild på platsen för en cell vars rad- och kolumnindex är 1 i kalkylbladet. Det är cellen "B2".
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Hämta det infogade bildobjektet
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Ange bildens ramfärg
if (pic.GetBorderLineColor() == Color{ 0xff, 0, 0, 0xff })//Blue
{
    pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
}
//Spara Excel-filen.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
