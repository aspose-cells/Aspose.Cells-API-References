---
title: "LineFormat.EndArrowheadStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Obtiene y establece el tipo de flecha final de la línea"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/endarrowheadstyle/
---
## LineFormat.EndArrowheadStyle property

Obtiene y establece el tipo de flecha final de la línea.

```csharp
public MsoArrowheadStyle EndArrowheadStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyEndArrowheadStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Obtener el formato de línea
            LineFormat lineFmt = line.Line;

            // Establece el estilo de la flecha final
            lineFmt.EndArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatPropertyEndArrowheadStyleDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


