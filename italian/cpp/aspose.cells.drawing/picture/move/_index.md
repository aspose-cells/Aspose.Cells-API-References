---
title: Aspose::Cells::Drawing::Picture::Move method
linktitle: Move
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Move method. Moves the picture to a specified location in C++.'
type: docs
weight: 700
url: /it/cpp/aspose.cells.drawing/picture/move/
---
## Picture::Move method


Moves the picture to a specified location.

```cpp
void Aspose::Cells::Drawing::Picture::Move(int32_t topRow, int32_t leftColumn)
```


| Parameter | Type | Description |
| --- | --- | --- |
| topRow | int32_t | Upper left row index. |
| leftColumn | int32_t | Upper left column index. |


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
//Imposta la nuova posizione dell'immagine
pic.Move(2, 4);
//Salva il file Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
