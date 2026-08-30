---
title: Aspose::Cells::Drawing::Picture::GetData method
linktitle: GetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetData method. Gets the data of the picture in C++.'
type: docs
weight: 1500
url: /fr/cpp/aspose.cells.drawing/picture/getdata/
---
## Picture::GetData method


Gets the data of the picture.

```cpp
Vector<uint8_t> Aspose::Cells::Drawing::Picture::GetData()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanciation d'un objet Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//insérer la première image
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//Obtenir l'objet image inséré
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//insérer la deuxième image
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//Obtenir l'objet image inséré
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Attribuer les données octet de la première image à la deuxième image
pic2.SetData(pic1.GetData());
//Enregistrez le fichier Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
