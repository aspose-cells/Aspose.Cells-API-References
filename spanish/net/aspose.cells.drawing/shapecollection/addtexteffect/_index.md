---
title: "ShapeCollection.AddTextEffect"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Método ShapeCollection. Inserta un objeto WordArt"
type: docs
url: /es/net/aspose.cells.drawing/shapecollection/addtexteffect/
---
## ShapeCollection.AddTextEffect method

Inserta un objeto WordArt.

```csharp
public Shape AddTextEffect(MsoPresetTextEffect effect, string text, string fontName, int size, 
    bool fontBold, bool fontItalic, int topRow, int top, int leftColumn, int left, int height, 
    int width)
```

| Parámetro | Tipo | Descripción |
| --- | --- | --- |
| efecto | MsoPresetTextEffect | El tipo de efecto de texto predefinido mso. |
| texto | String | El texto WordArt. |
| fontName | String | El nombre de la fuente. |
| tamaño | Int32 | El tamaño de la fuente |
| fontBold | Booleano | Indica si la fuente está en negrita. |
| fontItalic | Booleano | Indica si la fuente está en cursiva. |
| topRow | Int32 | Índice de fila superior izquierda. |
| superior | Int32 | Representa el desplazamiento vertical de la forma desde su fila izquierda, en unidades de píxel. |
| leftColumn | Int32 | Índice de columna superior izquierda. |
| izquierda | Int32 | Representa el desplazamiento horizontal de la forma desde su columna izquierda, en unidades de píxel. |
| altura | Int32 | Representa la altura de la forma, en unidades de píxel. |
| ancho | Int32 | Representa el ancho de la forma, en unidades de píxel. |

### Valor de retorno

Devuelve un objeto Shape que representa el nuevo objeto WordArt.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ShapeCollectionMethodAddTextEffectWithMsoPresetTextEffectStringStrinDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            ShapeCollection shapes = worksheet.Shapes;

            Shape wordArt = shapes.AddTextEffect(
                MsoPresetTextEffect.TextEffect10,
                "Sample WordArt",
                "Arial",
                18,
                false,
                false,
                3,
                0,
                3,
                0,
                200,
                50
            );

            workbook.Save("WordArtDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Shape](../../shape/)
* enum [MsoPresetTextEffect](../../msopresettexteffect/)
* class [ShapeCollection](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


