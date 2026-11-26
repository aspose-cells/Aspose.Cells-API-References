---
title: "MsoLineFormat.BackColor"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormat. Obtiene y establece el color de fondo de la línea del borde"
type: docs
url: /es/net/aspose.cells.drawing/msolineformat/backcolor/
---
## MsoLineFormat.BackColor property

Obtiene y establece el color de fondo de la línea del borde.

```csharp
public Color BackColor { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyBackColorDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            Shape line = worksheet.Shapes.AddLine(1, 1, 100, 100, 5, 5);

            // Establecer propiedades de línea
            line.LineFormat.ForeColor = Color.Red;
            line.LineFormat.BackColor = Color.Yellow; // Demonstrating BackColor usage
            line.LineFormat.DashStyle = MsoLineDashStyle.Solid;
            line.LineFormat.Weight = 2.0;

            // Guarda el libro de trabajo
            workbook.Save("LineFormatBackColorDemo.xlsx");
        }
    }
}
```

### Ver también

* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


