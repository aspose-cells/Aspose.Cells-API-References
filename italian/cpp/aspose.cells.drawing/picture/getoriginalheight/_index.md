---
title: Aspose::Cells::Drawing::Picture::GetOriginalHeight method
linktitle: GetOriginalHeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalHeight method. Gets the original height of the picture in C++.'
type: docs
weight: 1100
url: /it/cpp/aspose.cells.drawing/picture/getoriginalheight/
---
## Picture::GetOriginalHeight method


Gets the original height of the picture.

```cpp
int32_t Aspose::Cells::Drawing::Picture::GetOriginalHeight()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Istanziare un oggetto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Aggiunta di un'immagine nella posizione di una cella i cui indici di riga e colonna sono 1 nel foglio di lavoro. È la cella "B2"
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Ottieni l'oggetto immagine inserito
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Restituisce l'altezza originale dell'immagine.
int picHeight = pic.GetOriginalHeight();
//Salva il file Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
