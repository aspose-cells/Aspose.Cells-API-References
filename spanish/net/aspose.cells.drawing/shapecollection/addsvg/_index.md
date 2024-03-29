---
title: AddSvg
second_title: Referencia de API de Aspose.Cells para .NET
description: Agrega imagen svg.
type: docs
weight: 300
url: /es/net/aspose.cells.drawing/shapecollection/addsvg/
---
## ShapeCollection.AddSvg method

Agrega imagen svg.

```csharp
public Picture AddSvg(int upperLeftRow, int top, int upperLeftColumn, int left, int height, 
    int width, byte[] svgData, byte[] compatibleImageData)
```

| Parámetro | Escribe | Descripción |
| --- | --- | --- |
| upperLeftRow | Int32 | Índice de la fila superior izquierda. |
| top | Int32 | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| upperLeftColumn | Int32 | Índice de la columna superior izquierda. |
| left | Int32 | El desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| height | Int32 | La altura de la forma, en unidades de píxel. |
| width | Int32 | El ancho de la forma, en unidades de píxel. |
| svgData | Byte[] | Los datos de la imagen svg. |
| compatibleImageData | Byte[] | Datos de imagen convertidos de svg para que sean compatibles con Excel 2016 o versiones inferiores. |

### Ejemplos

```csharp

[C#]
// agregar un svg
using (FileStream fs = new FileStream("image.svg", FileMode.Open))
{
    int len = (int)fs.Length;
    byte[] imageData = new byte[len];
    fs.Read(imageData, 0, len);
    Picture picture = shapes.AddSvg(4, 0, 5, 0, -1, -1, imageData, null);
}
```

### Ver también

* class [Picture](../../picture)
* class [ShapeCollection](../../shapecollection)
* espacio de nombres [Aspose.Cells.Drawing](../../shapecollection)
* asamblea [Aspose.Cells](../../../)

<!-- DO NOT EDIT: generated by xmldocmd for Aspose.Cells.dll -->
