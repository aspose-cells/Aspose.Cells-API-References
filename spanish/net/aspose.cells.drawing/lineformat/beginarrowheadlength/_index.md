---
title: "LineFormat.BeginArrowheadLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Obtiene y establece el tipo de longitud de la flecha inicial de la línea"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/beginarrowheadlength/
---
## LineFormat.BeginArrowheadLength property

Obtiene y establece el tipo de longitud de la flecha inicial de la línea.

```csharp
public MsoArrowheadLength BeginArrowheadLength { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            Shape lineShape = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);
            LineShape line = (LineShape)lineShape;

            // Establecer la longitud de la punta de flecha inicial
            line.Line.BeginArrowheadLength = MsoArrowheadLength.Long;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatPropertyBeginArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


