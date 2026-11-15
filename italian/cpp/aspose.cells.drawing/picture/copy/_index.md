---
title: Aspose::Cells::Drawing::Picture::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
type: docs
weight: 600
url: /it/cpp/aspose.cells.drawing/picture/copy/
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
//Istanziare un oggetto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//inserisci la prima immagine
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Ottieni l'oggetto immagine inserito
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//inserisci la seconda immagine
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Ottieni l'oggetto immagine inserito
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Copia l'immagine 1 nell'immagine 2.Otterrai due oggetti immagine 1 sovrapposti l'uno sull'altro.
CopyOptions opt;
pic2.Copy(pic1, opt);
//Salva il file Excel.
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
