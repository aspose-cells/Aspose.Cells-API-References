---
title: "MsoLineFormat.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad MsoLineFormat. Devuelve un objeto Style que representa el estilo del rango especificado"
type: docs
url: /es/net/aspose.cells.drawing/msolineformat/style/
---
## MsoLineFormat.Style property

Devuelve un objeto Style que representa el estilo del rango especificado.

```csharp
public MsoLineStyle Style { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class MsoLineFormatPropertyStyleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar una forma de línea
            Aspose.Cells.Drawing.LineShape line = worksheet.Shapes.AddLine(5, 5, 100, 150, 10, 10);

            // Obtener el formato de línea
            MsoLineFormat lineFormat = line.LineFormat;

            // Establecer propiedades de estilo de línea
            lineFormat.Style = MsoLineStyle.ThickBetweenThin;
            lineFormat.ForeColor = System.Drawing.Color.Red;
            lineFormat.BackColor = System.Drawing.Color.White;
            lineFormat.DashStyle = MsoLineDashStyle.DashDotDot;
            lineFormat.Transparency = 0.5;
            lineFormat.Weight = 3.0;

            // Crear otra línea para comparación
            Aspose.Cells.Drawing.LineShape line2 = worksheet.Shapes.AddLine(5, 25, 100, 150, 10, 10);
            MsoLineFormat lineFormat2 = line2.LineFormat;

            // Copiar estilo de la primera línea a la segunda línea
            lineFormat2.Style = lineFormat.Style;
            lineFormat2.ForeColor = lineFormat.ForeColor;
            lineFormat2.BackColor = lineFormat.BackColor;
            lineFormat2.DashStyle = lineFormat.DashStyle;
            lineFormat2.Transparency = lineFormat.Transparency;
            lineFormat2.Weight = lineFormat.Weight;

            // Guarda el libro de trabajo
            workbook.Save("MsoLineFormatStyleDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoLineStyle](../../msolinestyle/)
* class [MsoLineFormat](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


