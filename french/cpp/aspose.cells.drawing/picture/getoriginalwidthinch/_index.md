---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidthInch method
linktitle: GetOriginalWidthInch
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidthInch method. Gets the original width of picture, in unit of inches in C++.'
type: docs
weight: 3300
url: /fr/cpp/aspose.cells.drawing/picture/getoriginalwidthinch/
---
## Picture::GetOriginalWidthInch method


Gets the original width of picture, in unit of inches.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalWidthInch()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanciation d'un objet Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Ajout d'une image à l'emplacement d'une cellule dont les indices de ligne et de colonne sont 1 dans la feuille de calcul. Il s'agit de la cellule "B2".
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Obtenir l'objet image inséré
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Obtient la largeur originale de l'image.
double picWidthInch = pic.GetOriginalWidthInch();
//Enregistrez le fichier Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
