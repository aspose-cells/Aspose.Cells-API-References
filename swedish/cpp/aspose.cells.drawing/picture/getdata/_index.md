---
title: Aspose::Cells::Drawing::Picture::GetData method
linktitle: GetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetData method. Gets the data of the picture in C++.'
type: docs
weight: 1500
url: /sv/cpp/aspose.cells.drawing/picture/getdata/
---
## Picture::GetData method


Gets the data of the picture.

```cpp
Vector<uint8_t> Aspose::Cells::Drawing::Picture::GetData()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instansierar ett Workbook‑objekt
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//infoga första bilden
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//Hämta det infogade bildobjektet
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//infoga andra bilden
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//Hämta det infogade bildobjektet
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Tilldela byte-data från den första bilden till den andra bilden
pic2.SetData(pic1.GetData());
//Spara Excel-filen.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
