---
title: Aspose::Cells::Drawing::Picture::GetOriginalHeightCM method
linktitle: GetOriginalHeightCM
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalHeightCM method. Gets the original height of picture, in unit of centimeters in C++.'
type: docs
weight: 3000
url: /fr/cpp/aspose.cells.drawing/picture/getoriginalheightcm/
---
## Picture::GetOriginalHeightCM method


Gets the original height of picture, in unit of centimeters.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalHeightCM()
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
//Obtient la hauteur originale de l'image.
double picHeightCM = pic.GetOriginalHeightCM();
//Enregistrez le fichier Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
