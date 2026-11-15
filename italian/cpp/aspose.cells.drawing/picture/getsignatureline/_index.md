---
title: Aspose::Cells::Drawing::Picture::GetSignatureLine method
linktitle: GetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3600
url: /it/cpp/aspose.cells.drawing/picture/getsignatureline/
---
## Picture::GetSignatureLine method


Gets and sets the signature line.

```cpp
SignatureLine Aspose::Cells::Drawing::Picture::GetSignatureLine()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Istanziare un oggetto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Aggiunta di un'immagine nella posizione di una cella i cui indici di riga e colonna sono 1 nel foglio di lavoro. È la cella "B2"
int imgIndex = worksheet.GetPictures().Add(1, 1, Vector<uint8_t>(0));
//Ottieni l'oggetto immagine inserito
Picture pic = worksheet.GetPictures().Get(imgIndex);
// Crea oggetto linea di firma
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// Assegna l'oggetto linea di firma a Picture.
pic.SetSignatureLine(s);

SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
    //fai quello che vuoi
}
//Salva il file Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
