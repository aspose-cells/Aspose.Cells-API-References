---
title: ImageType
second_title: Referencia de API de Aspose.Cells para .NET
description: Obtiene el formato de imagen de la imagen.
type: docs
weight: 60
url: /es/net/aspose.cells.drawing/picture/imagetype/
---
## Picture.ImageType property

Obtiene el formato de imagen de la imagen.

```csharp
public ImageType ImageType { get; }
```

### Ejemplos

```csharp

[C#]
// Instanciando un objeto Workbook
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.Worksheets[0];
//insertar primera imagen
int imgIndex1 = worksheet.Pictures.Add(1, 1, "1.png");
//Obtener el objeto de imagen insertado
Picture pic1 = worksheet.Pictures[imgIndex1];
if(pic1.ImageType == Aspose.Cells.Drawing.ImageType.Png)
{
    //El tipo de imagen es png.";
}
//insertar segunda imagen
int imgIndex2 = worksheet.Pictures.Add(1, 9, "2.jpeg");
//Obtener el objeto de imagen insertado
Picture pic2 = worksheet.Pictures[imgIndex2];
if(pic2.ImageType == Aspose.Cells.Drawing.ImageType.Jpeg)
{
    //El tipo de imagen es jpg.";
}
```

### Ver también

* enum [ImageType](../../imagetype)
* class [Picture](../../picture)
* espacio de nombres [Aspose.Cells.Drawing](../../picture)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->