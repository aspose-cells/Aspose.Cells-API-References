---
title: Aspose::Cells::Drawing::Picture::SetBorderWeight method
linktitle: SetBorderWeight
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetBorderWeight method. Gets or sets the weight of the border line of a picture in units of pt in C++.'
type: docs
weight: 1400
url: /es/cpp/aspose.cells.drawing/picture/setborderweight/
---
## Picture::SetBorderWeight method


Gets or sets the weight of the border line of a picture in units of pt.

```cpp
void Aspose::Cells::Drawing::Picture::SetBorderWeight(double value)
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
//Establecer el color del borde de la imagen
pic.SetBorderLineColor(Color{ 0xff, 0xff, 0, 0 });//Red
//Establecer el ancho del borde de la imagen
if (pic.GetBorderWeight() == 3)
{
    pic.SetBorderWeight(3);
}
//Guarde el archivo de Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
