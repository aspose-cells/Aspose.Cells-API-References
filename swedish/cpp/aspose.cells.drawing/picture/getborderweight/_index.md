---
title: Aspose::Cells::Drawing::Picture::GetBorderWeight method
linktitle: GetBorderWeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
type: docs
weight: 1300
url: /sv/cpp/aspose.cells.drawing/picture/getborderweight/
---
## Picture::GetBorderWeight method


Gets or sets the weight of the border line of a picture in units of pt.

```cpp
double Aspose::Cells::Drawing::Picture::GetBorderWeight()
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
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Ange bildens rambredd
if (pic.GetBorderWeight() == 3)
{
    pic.SetBorderWeight(3);
}
//Spara Excel-filen.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
