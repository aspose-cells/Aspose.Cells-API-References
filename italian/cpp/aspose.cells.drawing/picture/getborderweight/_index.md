---
title: Aspose::Cells::Drawing::Picture::GetBorderWeight method
linktitle: GetBorderWeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
type: docs
weight: 1500
url: /it/cpp/aspose.cells.drawing/picture/getborderweight/
---
## Picture::GetBorderWeight method


Gets or sets the weight of the border line of a picture in units of pt.

```cpp
double Aspose::Cells::Drawing::Picture::GetBorderWeight()
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
//Imposta il colore del bordo dell'immagine
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Imposta la larghezza del bordo dell'immagine
if (pic.GetBorderWeight() == 3)
{
    pic.SetBorderWeight(3);
}
//Salva il file Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
