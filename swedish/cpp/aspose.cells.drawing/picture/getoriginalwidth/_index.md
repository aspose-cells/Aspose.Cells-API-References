---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidth method
linktitle: GetOriginalWidth
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidth method. Gets the original width of the picture in C++.'
type: docs
weight: 1000
url: /sv/cpp/aspose.cells.drawing/picture/getoriginalwidth/
---
## Picture::GetOriginalWidth method


Gets the original width of the picture.

```cpp
int32_t Aspose::Cells::Drawing::Picture::GetOriginalWidth()
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
//Hämtar bildens ursprungliga bredd.
int picWidth = pic.GetOriginalWidth();
//Spara Excel-filen.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
