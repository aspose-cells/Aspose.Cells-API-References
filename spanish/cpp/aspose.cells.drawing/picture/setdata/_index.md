---
title: Aspose::Cells::Drawing::Picture::SetData method
linktitle: SetData
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetData method. Gets the data of the picture in C++.'
type: docs
weight: 1600
url: /es/cpp/aspose.cells.drawing/picture/setdata/
---
## Picture::SetData method


Gets the data of the picture.

```cpp
void Aspose::Cells::Drawing::Picture::SetData(const Vector<uint8_t> &value)
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanciando un objeto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//insertar la primera imagen
int imgIndex1 = worksheet.GetPictures().Add(1, 1, u"example1.png");
//Obtener el objeto de imagen insertado
Picture pic1 = worksheet.GetPictures().Get(imgIndex1);
//insertar la segunda imagen
int imgIndex2 = worksheet.GetPictures().Add(1, 9, u"example2.jpeg");
//Obtener el objeto de imagen insertado
Picture pic2 = worksheet.GetPictures().Get(imgIndex2);
//Asignar los datos de bytes de la primera imagen a la segunda imagen
pic2.SetData(pic1.GetData());
//Guarde el archivo de Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
