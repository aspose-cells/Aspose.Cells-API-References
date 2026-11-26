---
title: "ShapeCollection.AddWordArt"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Añade WordArt predefinido desde Excel 2007."
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addwordart/
---
## ShapeCollection.AddWordArt method

Agrega WordArt predefinido desde Excel 2007.

```csharp
public Shape AddWordArt(PresetWordArtStyle style, string text, int topRow, int top, int leftColumn, 
    int left, int height, int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| estilo | PresetWordArtStyle | El estilo predefinido de WordArt. |
| texto | String | El texto. |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura de la forma, en unidades de píxel. |
| ancho | Int32 | Representa el ancho de la forma, en unidades de píxel. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddWordArtWithPresetWordArtStyleStringInt32IDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Obtener la colección de formas
            ShapeCollection shapes = worksheet.Shapes;

            // Agregar un WordArt con parámetros especificados
            Shape wordArt = shapes.AddWordArt(
                PresetWordArtStyle.WordArtStyle1, 
                "Sample WordArt", 
                10,  // left
                10,  // top
                200, // width
                50,  // height
                100, // rotation
                200  // z-order
            );

            // Guarda el libro de trabajo
            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [PresetWordArtStyle](../../presetwordartstyle/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


