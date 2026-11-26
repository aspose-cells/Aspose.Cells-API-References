---
title: "Enumeración LineCapType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enumeración Aspose.Cells.Drawing.LineCapType. Representa los extremos de una línea"
type: docs
url: /es/net/aspose.cells.drawing/linecaptype/
---
## LineCapType enumeration

Representa los extremos de una línea

```csharp
public enum LineCapType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Square | `0` | Cuadrado sobresale por la mitad del ancho de línea. |
| Round | `1` | Extremos redondeados. |
| Flat | `2` | La línea termina en el punto final. |
| None | `3` | Sin tapa |

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class DrawingClassLineCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Shape shape = worksheet.Shapes.AddRectangle(1, 0, 1, 0, 50, 100);
            
            LineFormat lineFmt = shape.Line;
            lineFmt.CapType = LineCapType.Flat;
            lineFmt.Weight = 2.0;
            lineFmt.DashStyle = MsoLineDashStyle.Solid;
            
            workbook.Save("LineCapTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Drawing](../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../)


