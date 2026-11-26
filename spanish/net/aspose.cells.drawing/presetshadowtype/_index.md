---
title: "Enum PresetShadowType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Drawing.PresetShadowType. Representa el tipo de sombra predefinida"
type: docs
url: /es/net/aspose.cells.drawing/presetshadowtype/
---
## PresetShadowType enumeration

Representa el tipo de sombra preestablecido.

```csharp
public enum PresetShadowType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| NoShadow | `0` | Sin sombra. |
| Custom | `1` | Sombra personalizada. |
| OffsetDiagonalBottomRight | `2` | Desplazamiento de sombra externa diagonal abajo a la derecha. |
| OffsetBottom | `3` | Desplazamiento de sombra externa abajo. |
| OffsetDiagonalBottomLeft | `4` | Desplazamiento de sombra externa diagonal inferior izquierda. |
| OffsetRight | `5` | Desplazamiento de sombra externa a la derecha. |
| OffsetCenter | `6` | Desplazamiento de sombra externa al centro. |
| OffsetLeft | `7` | Desplazamiento de sombra externa a la izquierda. |
| OffsetDiagonalTopRight | `8` | Desplazamiento de sombra externa diagonal superior derecha. |
| OffsetTop | `9` | Desplazamiento de sombra externa en la parte superior. |
| OffsetDiagonalTopLeft | `10` | Desplazamiento de sombra externa diagonal superior izquierda. |
| InsideDiagonalTopLeft | `11` | Sombra interna dentro de diagonal superior izquierda. |
| InsideTop | `12` | Sombra interna en la parte superior. |
| InsideDiagonalTopRight | `13` | Sombra interna dentro de diagonal superior derecha. |
| InsideLeft | `14` | Sombra interna a la izquierda. |
| InsideCenter | `15` | Sombra interna en el centro. |
| InsideRight | `16` | Sombra interna a la derecha. |
| InsideDiagonalBottomLeft | `17` | Sombra interna dentro de diagonal inferior izquierda. |
| InsideBottom | `18` | Sombra interna en la parte inferior. |
| InsideDiagonalBottomRight | `19` | Sombra interna dentro de diagonal inferior derecha. |
| PerspectiveDiagonalUpperLeft | `20` | Sombra externa en perspectiva diagonal superior izquierda. |
| PerspectiveDiagonalUpperRight | `21` | Sombra externa en perspectiva diagonal superior derecha. |
| Below | `22` | Sombra externa debajo. |
| PerspectiveDiagonalLowerLeft | `23` | Sombra externa en perspectiva diagonal inferior izquierda. |
| PerspectiveDiagonalLowerRight | `24` | Sombra externa en perspectiva diagonal inferior derecha. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassPresetShadowTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Añadir una forma para demostrar los efectos de sombra
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 100, 100);
            
            // Establecer diferentes tipos de sombra predefinidos
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetDiagonalBottomRight;
            Console.WriteLine("Shadow type set to: " + shape.ShadowEffect.PresetType);

            // Cambiar a otro tipo de sombra
            shape.ShadowEffect.PresetType = PresetShadowType.OffsetBottom;
            Console.WriteLine("Shadow type changed to: " + shape.ShadowEffect.PresetType);

            // Guarda el libro de trabajo
            workbook.Save("PresetShadowTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


