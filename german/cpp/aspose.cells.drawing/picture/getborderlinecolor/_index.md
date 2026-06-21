---
title: Aspose::Cells::Drawing::Picture::GetBorderLineColor method
linktitle: GetBorderLineColor
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetBorderLineColor method. Represents the Color of the border line of a picture in C++.'
type: docs
weight: 1100
url: /de/cpp/aspose.cells.drawing/picture/getborderlinecolor/
---
## Picture::GetBorderLineColor method


Represents the [Color](../../../aspose.cells/color/) of the border line of a picture.

```cpp
Aspose::Cells::Color Aspose::Cells::Drawing::Picture::GetBorderLineColor()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Ein Bild an der Position einer Zelle hinzufügen, deren Zeilen‑ und Spaltenindizes 1 sind, im Arbeitsblatt. Es ist die Zelle "B2".
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Das eingefügte Bildobjekt abrufen
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Die Rahmenfarbe des Bildes festlegen
if (pic.GetBorderLineColor() == Color{ 0xff, 0, 0, 0xff })//Blue
{
    pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
}
//Speichern Sie die Excel-Datei.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
