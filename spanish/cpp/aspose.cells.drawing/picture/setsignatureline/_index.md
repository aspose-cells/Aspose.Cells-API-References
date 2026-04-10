---
title: Aspose::Cells::Drawing::Picture::SetSignatureLine method
linktitle: SetSignatureLine
second_title: Aspose.Cells for C++ API Reference
description: 'Aspose::Cells::Drawing::Picture::SetSignatureLine method. Gets and sets the signature line in C++.'
type: docs
weight: 3500
url: /es/cpp/aspose.cells.drawing/picture/setsignatureline/
---
## Picture::SetSignatureLine method


Gets and sets the signature line.

```cpp
void Aspose::Cells::Drawing::Picture::SetSignatureLine(const SignatureLine &value)
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
// Crear objeto de línea de firma
SignatureLine s;
s.SetSigner(u"Simon Zhao");
s.SetTitle(u"Development Lead");
s.SetEmail(u"Simon.Zhao@aspose.com");
// Asignar el objeto de línea de firma a Picture.
pic.SetSignatureLine(s);

SignatureLine s2 = pic.GetSignatureLine();
if (s2.GetSigner() == s.GetSigner())
{
    //haz lo que quieras
}
//Guarde el archivo de Excel.
workbook.Save(u"result.xlsx");
Aspose::Cells::Cleanup();
```

## See Also

* Class [Vector](../../../aspose.cells/vector/)
* Class [SignatureLine](../../signatureline/)
* Class [Picture](../)
* Namespace [Aspose::Cells::Drawing](../../)
* Library [Aspose.Cells for C++](../../../)
