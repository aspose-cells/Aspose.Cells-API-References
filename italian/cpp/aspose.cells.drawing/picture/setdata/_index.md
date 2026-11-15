---
title: Aspose::Cells::Drawing::Picture::SetData method
linktitle: SetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetData method. Gets the data of the picture in C++.'
type: docs
weight: 1800
url: /it/cpp/aspose.cells.drawing/picture/setdata/
---
## Picture::SetData method


Gets the data of the picture.

```cpp
void Aspose::Cells::Drawing::Picture::SetData(const Vector<uint8_t> &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Istanziare un oggetto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//inserisci la prima immagine
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//Ottieni l'oggetto immagine inserito
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//inserisci la seconda immagine
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//Ottieni l'oggetto immagine inserito
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Assegna i dati byte della prima immagine alla seconda immagine
pic2.SetData(pic1.GetData());
//Salva il file Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
