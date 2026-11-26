---
title: "LineFormat.EndArrowheadWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Obtiene y establece el tipo de ancho de flecha final de la línea"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/endarrowheadwidth/
---
## LineFormat.EndArrowheadWidth property

Obtiene y establece el tipo de ancho de la flecha final de la línea.

```csharp
public MsoArrowheadWidth EndArrowheadWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadWidthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            Shape line = worksheet.Shapes.AddLine(10, 10, 100, 10, 5, 5);

            // Obtener el formato de línea
            LineFormat lineFmt = line.Line;

            // Establecer el ancho de la flecha final
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatPropertyEndArrowheadWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


