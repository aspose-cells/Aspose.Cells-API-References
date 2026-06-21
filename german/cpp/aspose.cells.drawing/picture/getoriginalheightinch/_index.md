---
title: Aspose::Cells::Drawing::Picture::GetOriginalHeightInch method
linktitle: GetOriginalHeightInch
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalHeightInch method. Gets the original height of picture, in unit of inches in C++.'
type: docs
weight: 3200
url: /de/cpp/aspose.cells.drawing/picture/getoriginalheightinch/
---
## Picture::GetOriginalHeightInch method


Gets the original height of picture, in unit of inches.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalHeightInch()
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
//Gibt die ursprüngliche Höhe des Bildes zurück.
double picHeightInch = pic.GetOriginalHeightInch();
//Speichern Sie die Excel-Datei.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
