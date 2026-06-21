---
title: Aspose::Cells::Drawing::Picture::GetData method
linktitle: GetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetData method. Gets the data of the picture in C++.'
type: docs
weight: 1500
url: /de/cpp/aspose.cells.drawing/picture/getdata/
---
## Picture::GetData method


Gets the data of the picture.

```cpp
Vector<uint8_t> Aspose::Cells::Drawing::Picture::GetData()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//erstes Bild einfügen
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//Das eingefügte Bildobjekt abrufen
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//zweites Bild einfügen
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//Das eingefügte Bildobjekt abrufen
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Weise die Byte-Daten des ersten Bildes dem zweiten Bild zu
pic2.SetData(pic1.GetData());
//Speichern Sie die Excel-Datei.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
