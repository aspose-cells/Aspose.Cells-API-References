---
title: Aspose::Cells::Drawing::Picture::Move method
linktitle: Move
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Move method. Moves the picture to a specified location in C++.'
type: docs
weight: 700
url: /fr/cpp/aspose.cells.drawing/picture/move/
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
//Instanciation d'un objet Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Ajout d'une image à l'emplacement d'une cellule dont les indices de ligne et de colonne sont 1 dans la feuille de calcul. Il s'agit de la cellule "B2".
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Obtenir l'objet image inséré
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Définir le nouvel emplacement de l'image
pic.Move(2, 4);
//Enregistrez le fichier Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
