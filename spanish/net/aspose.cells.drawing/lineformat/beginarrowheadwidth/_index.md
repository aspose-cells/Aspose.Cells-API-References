---
title: "LineFormat.BeginArrowheadWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Obtiene y establece el tipo de ancho de flecha inicial de la línea"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/beginarrowheadwidth/
---
## LineFormat.BeginArrowheadWidth property

Obtiene y establece el tipo de ancho de la flecha inicial de la línea.

```csharp
public MsoArrowheadWidth BeginArrowheadWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Establecer las propiedades del formato de línea
            LineFormat lineFmt = line.Line;
            lineFmt.BeginArrowheadWidth = MsoArrowheadWidth.Medium;
            lineFmt.EndArrowheadWidth = MsoArrowheadWidth.Medium;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


