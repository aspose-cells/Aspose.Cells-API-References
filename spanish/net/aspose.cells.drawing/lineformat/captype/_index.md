---
title: "LineFormat.CapType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Especifica los extremos finales"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/captype/
---
## LineFormat.CapType property

Especifica los extremos finales.

```csharp
public LineCapType CapType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCapTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Establecer propiedades del formato de línea
            LineFormat lineFmt = line.Line;
            lineFmt.CapType = LineCapType.Flat;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatCapTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [LineCapType](../../linecaptype/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


