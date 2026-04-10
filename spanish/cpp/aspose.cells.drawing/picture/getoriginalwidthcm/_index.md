---
title: Aspose::Cells::Drawing::Picture::GetOriginalWidthCM method
linktitle: GetOriginalWidthCM
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::GetOriginalWidthCM method. Gets the original width of picture, in unit of centimeters in C++.'
type: docs
weight: 3100
url: /es/cpp/aspose.cells.drawing/picture/getoriginalwidthcm/
---
## Picture::GetOriginalWidthCM method


Gets the original width of picture, in unit of centimeters.

```cpp
double Aspose::Cells::Drawing::Picture::GetOriginalWidthCM()
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
double picWidthCM = pic.GetOriginalWidthCM();
//Guarde el archivo de Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
