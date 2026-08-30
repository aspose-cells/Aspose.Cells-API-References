---
title: Aspose::Cells::Drawing::Picture::GetOriginalHeight method
linktitle: GetOriginalHeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalHeight method. Gets the original height of the picture in C++.'
type: docs
weight: 1100
url: /fr/cpp/aspose.cells.drawing/picture/getoriginalheight/
---
## Picture::GetOriginalHeight method


Gets the original height of the picture.

```cpp
int32_t Aspose::Cells::Drawing::Picture::GetOriginalHeight()
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
int picHeight = pic.GetOriginalHeight();
//Enregistrez le fichier Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
