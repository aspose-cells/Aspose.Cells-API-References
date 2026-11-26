---
title: "LineFormat.CompoundType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Especifica el tipo compuesto de la línea"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/compoundtype/
---
## LineFormat.CompoundType property

Especifica el tipo compuesto de la línea.

```csharp
public MsoLineStyle CompoundType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyCompoundTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Obtener el formato de línea
            LineFormat lineFmt = line.Line;

            // Establecer tipo compuesto
            lineFmt.CompoundType = MsoLineStyle.Single;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatCompoundTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoLineStyle](../../msolinestyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


