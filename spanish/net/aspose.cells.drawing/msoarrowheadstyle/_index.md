---
title: "Enumeración MsoArrowheadStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.MsoArrowheadStyle. Enumera el tipo de extremo de línea del borde de la forma"
type: docs
url: /es/net/aspose.cells.drawing/msoarrowheadstyle/
---
## MsoArrowheadStyle enumeration

Enumera el tipo de extremo de línea del borde de la forma.

```csharp
public enum MsoArrowheadStyle
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| None | `0` | Sin tipo de extremo de línea. |
| Arrow | `1` | Tipo de extremo de línea de flecha. |
| ArrowStealth | `2` | Tipo de extremo de línea de flecha sigilosa. |
| ArrowDiamond | `3` | Tipo de extremo de línea de flecha diamante. |
| ArrowOval | `4` | Tipo de extremo de línea de flecha ovalada. |
| ArrowOpen | `5` | Tipo de extremo de línea de flecha abierta. |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassMsoArrowheadStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            LineShape lineShape = worksheet.Shapes.AddLine(5, 5, 10, 10, 100, 100);

            // Establecer propiedades de línea
            MsoLineFormat lineFormat = lineShape.LineFormat;
            lineFormat.ForeColor = System.Drawing.Color.Black;
            lineFormat.DashStyle = MsoLineDashStyle.DashDot;
            lineFormat.Weight = 0.75;

            // Establecer estilos de punta de flecha
            lineShape.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowStealth;
            lineShape.Line.EndArrowheadStyle = MsoArrowheadStyle.Arrow;
            lineShape.Line.BeginArrowheadLength = MsoArrowheadLength.Medium;
            lineShape.Line.EndArrowheadLength = MsoArrowheadLength.Medium;

            // Guarda el libro de trabajo
            workbook.Save("MsoArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


