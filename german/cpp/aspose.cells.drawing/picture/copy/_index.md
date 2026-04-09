---
title: Aspose::Cells::Drawing::Picture::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
type: docs
weight: 600
url: /de/cpp/aspose.cells.drawing/picture/copy/
---
## Picture::Copy method


Copy the picture.

```cpp
void Aspose::Cells::Drawing::Picture::Copy(const Aspose::Cells::Drawing::Picture &source, const CopyOptions &options)
```


| Parameter | Type | Description |
| --- | --- | --- |
| source | const Aspose::Cells::Drawing::Picture\& | The source picture. |
| options | const CopyOptions\& | The copy options. |


## Examples


```cpp
Aspose::Cells::Startup();
//Instanziieren eines Workbook-Objekts
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//erstes Bild einfügen
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Das eingefügte Bildobjekt abrufen
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//zweites Bild einfügen
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Das eingefügte Bildobjekt abrufen
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Kopiere Bild 1 zu Bild 2. Sie erhalten zwei Bild‑1‑Objekte, die übereinander liegen.
CopyOptions opt;
pic2.Copy(pic1, opt);
//Speichern Sie die Excel-Datei.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Class [CopyOptions](../../../aspose.cells/copyoptions/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
