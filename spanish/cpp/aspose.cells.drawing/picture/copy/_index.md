---
title: Aspose::Cells::Drawing::Picture::Copy method
linktitle: Copy
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::Copy method. Copy the picture in C++.'
type: docs
weight: 600
url: /es/cpp/aspose.cells.drawing/picture/copy/
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
//Instanciando un objeto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//insertar la primera imagen
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"1.png");
//Obtener el objeto de imagen insertado
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//insertar la segunda imagen
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"2.jpeg");
//Obtener el objeto de imagen insertado
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Copiar la imagen 1 a la imagen 2. Obtendrá dos objetos de imagen 1 superpuestos uno sobre otro.
CopyOptions opt;
pic2.Copy(pic1, opt);
//Guarde el archivo de Excel.
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
