---
title: Aspose::Cells::Drawing::Picture::Move method
linktitle: Move
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Move method. Moves the picture to a specified location in C++.'
type: docs
weight: 700
url: /sv/cpp/aspose.cells.drawing/picture/move/
---
## Picture::Move method


Moves the picture to a specified location.

```cpp
void Aspose::Cells::Drawing::Picture::Move(int32_t topRow, int32_t leftColumn)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |


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
//Ange bildens nya plats
pic.Move(2, 4);
//Spara Excel-filen.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
