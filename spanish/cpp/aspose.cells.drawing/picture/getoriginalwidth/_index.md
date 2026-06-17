---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidth method
linktitle: GetOriginalWidth
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidth method. Gets the original width of the picture in C++.'
type: docs
weight: 1000
url: /es/cpp/aspose.cells.drawing/picture/getoriginalwidth/
---
## Picture::GetOriginalWidth method


Gets the original width of the picture.

```cpp
int32_t Aspose::Cells::Drawing::Picture::GetOriginalWidth()
```


## Examples


```cpp
Aspose::Cells::Startup();
//Instanciando un objeto Workbook
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Agregar una imagen en la ubicación de una celda cuyos índices de fila y columna son 1 en la hoja de cálculo. Es la celda "B2"
int imgIndex = worksheet.GetPictures().Add(1, 1, u"example.jpeg");
//Obtener el objeto de imagen insertado
Picture pic = worksheet.GetPictures().Get(imgIndex);
//Obtiene el ancho original de la imagen.
int picWidth = pic.GetOriginalWidth();
//Guarde el archivo de Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
