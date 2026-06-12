---
title: Aspose::Cells::Drawing::Picture::GetOriginalHeightCM method
linktitle: GetOriginalHeightCM
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalHeightCM method. Gets the original height of picture, in unit of centimeters in C++.'
type: docs
weight: 3000
url: /sv/cpp/aspose.cells.drawing/picture/getoriginalheightcm/
---
## Picture::GetOriginalHeightCM method


Gets the original height of picture, in unit of centimeters.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalHeightCM()
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
//Hämtar bildens ursprungliga höjd.
double picHeightCM = pic.GetOriginalHeightCM();
//Spara Excel-filen.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
