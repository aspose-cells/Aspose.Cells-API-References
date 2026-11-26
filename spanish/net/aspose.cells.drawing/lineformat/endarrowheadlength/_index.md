---
title: "LineFormat.EndArrowheadLength"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Obtiene y establece el tipo de longitud de la flecha final de la línea"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/endarrowheadlength/
---
## LineFormat.EndArrowheadLength property

Obtiene y establece el tipo de longitud de la flecha final de la línea.

```csharp
public MsoArrowheadLength EndArrowheadLength { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadLengthDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea y obtener el objeto de forma directamente
            LineShape line = (LineShape)worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 10);

            // Establecer la longitud de la punta de flecha final
            line.Line.EndArrowheadLength = MsoArrowheadLength.Long;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatPropertyEndArrowheadLengthDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadLength](../../msoarrowheadlength/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


