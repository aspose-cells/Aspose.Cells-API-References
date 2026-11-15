---
title: Aspose::Cells::Drawing::Picture::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
type: docs
weight: 600
url: /fr/cpp/aspose.cells.drawing/picture/copy/
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
//Instanciation d'un objet Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//insérer la première image
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Obtenir l'objet image inséré
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//insérer la deuxième image
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Obtenir l'objet image inséré
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Copier l'image 1 vers l'image 2. Vous obtiendrez deux objets image 1 superposés l'un sur l'autre.
CopyOptions opt;
pic2.Copy(pic1, opt);
//Enregistrez le fichier Excel.
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
