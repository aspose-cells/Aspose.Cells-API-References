---
title: "LineFormat.BeginArrowheadStyle"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad LineFormat. Obtiene y establece el tipo de flecha inicial de la línea"
type: docs
url: /es/net/aspose.cells.drawing/lineformat/beginarrowheadstyle/
---
## LineFormat.BeginArrowheadStyle property

Obtiene y establece el tipo de flecha inicial de la línea.

```csharp
public MsoArrowheadStyle BeginArrowheadStyle { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class LineFormatPropertyBeginArrowheadStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            Shape line = worksheet.Shapes.AddLine(5, 5, 100, 5, 10, 100);

            // Establecer el estilo de la punta de flecha inicial
            line.Line.BeginArrowheadStyle = MsoArrowheadStyle.ArrowOpen;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatPropertyBeginArrowheadStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadStyle](../../msoarrowheadstyle/)
* class [LineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


