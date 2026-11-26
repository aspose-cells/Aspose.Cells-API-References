---
title: "Enum PresetWordArtStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.PresetWordArtStyle. Representa los estilos de WordArt predefinidos"
type: docs
url: /es/net/aspose.cells.drawing/presetwordartstyle/
---
## PresetWordArtStyle enumeration

Representa los estilos de WordArt preestablecidos.

```csharp
public enum PresetWordArtStyle
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| WordArtStyle1 | `1` | Relleno - Negro, Texto 1, Sombra |
| WordArtStyle2 | `2` | Relleno - Azul, Acento 1, Sombra |
| WordArtStyle3 | `3` | Relleno - Naranja, Acento 2, Contorno - Acento 2 |
| WordArtStyle4 | `4` | Relleno - Blanco, Contorno - Acento 1, Sombra |
| WordArtStyle5 | `5` | Relleno - Oro, Acento 4, Bisel suave |
| WordArtStyle6 | `6` | Relleno degradado - Gris |
| WordArtStyle7 | `7` | Relleno degradado - Azul, Acento 1, Reflexión |
| WordArtStyle8 | `8` | Relleno degradado - Oro, Acento 4, Contorno - Acento 4 |
| WordArtStyle9 | `9` | Relleno - Blanco, Contorno - Acento 1, Resplandor - Acento 1 |
| WordArtStyle10 | `10` | Relleno - Gris-50%, Acento 3, Bisel agudo |
| WordArtStyle11 | `11` | Relleno - Negro, Texto 1, Contorno - Fondo 1, Sombra dura - Fondo 1 |
| WordArtStyle12 | `12` | Relleno - Negro, Texto 1, Contorno - Fondo 1, Sombra dura - Acento 1 |
| WordArtStyle13 | `13` | Relleno - Azul, Acento 1, Contorno - Fondo 1, Sombra dura - Acento 1 |
| WordArtStyle14 | `14` | Relleno - Blanco, Contorno - Acento 2, Sombra dura - Acento 2 |
| WordArtStyle15 | `15` | Relleno - Gris-25%, Fondo 2, Sombra interna |
| WordArtStyle16 | `16` | Relleno de patrón - Blanco, Texto 2, Diagonal ascendente oscura, Sombra |
| WordArtStyle17 | `17` | Relleno de patrón - Gris-50%, Acento 3, Horizontal estrecho, Sombra interna |
| WordArtStyle18 | `18` | Relleno - Azul, Acento 1, 50%, Sombra dura - Acento 1 |
| WordArtStyle19 | `19` | Relleno de patrón - Azul, Acento 1, Diagonal descendente clara, Contorno - Acento 1 |
| WordArtStyle20 | `20` | Relleno de patrón - Azul-gris, Texto 2, Diagonal ascendente oscura, Sombra dura - Texto 2 |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Drawing;
    using System;

    public class PresetWordArtStyleDemo
    {
        public static void PresetWordArtStyleExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Acceder a la primera hoja de cálculo
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Acceda a la colección de formas de la hoja de cálculo
            ShapeCollection shapes = worksheet.Shapes;
            
            // Agregue una forma WordArt con un estilo predefinido específico
            // Parámetros: style, text, upperLeftRow, top, upperLeftColumn, left, height, width
            Shape wordArt = shapes.AddWordArt(PresetWordArtStyle.WordArtStyle2, "Hello Aspose!", 1, 0, 1, 0, 100, 400);
            
            // Guarda el libro de trabajo
            workbook.Save("PresetWordArtStyleExample.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


