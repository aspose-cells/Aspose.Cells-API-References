---
title: Aspose::Cells::Drawing::Picture::SetBorderWeight method
linktitle: SetBorderWeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
type: docs
weight: 1400
url: /de/cpp/aspose.cells.drawing/picture/setborderweight/
---
## Picture::SetBorderWeight method


Gets or sets the weight of the border line of a picture in units of pt.

```cpp
void Aspose::Cells::Drawing::Picture::SetBorderWeight(double value)
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
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Die Rahmenbreite des Bildes festlegen
if (pic.GetBorderWeight() == 3)
{
    pic.SetBorderWeight(3);
}
//Speichern Sie die Excel-Datei.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
