---
title: Aspose::Cells::Drawing::Picture::GetSignatureLine method
linktitle: GetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3400
url: /fr/cpp/aspose.cells.drawing/picture/getsignatureline/
---
## Picture::GetSignatureLine method


Gets and sets the signature line.

```cpp
SignatureLine Aspose::Cells::Drawing::Picture::GetSignatureLine()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanciation d'un objet Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Ajout d'une image à l'emplacement d'une cellule dont les indices de ligne et de colonne sont 1 dans la feuille de calcul. Il s'agit de la cellule "B2".
int imgIndex = worksheet.GetPictures().Add(1, 1, Vector<uint8_t>(0));
//Obtenir l'objet image inséré
Picture pic = worksheet.GetPictures().Get(imgIndex);
// Créer un objet de ligne de signature
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// Attribuer l'objet ligne de signature à l'image.
pic.SetSignatureLine(s);

SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
    //faites ce que vous voulez
}
//Enregistrez le fichier Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
