---
title: "Line.EndArrowWidth"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Especifica el ancho de la punta de flecha para el final de una línea"
type: docs
url: /es/net/aspose.cells.drawing/line/endarrowwidth/
---
## Line.EndArrowWidth property

Especifica el ancho de la punta de flecha para el final de una línea.

```csharp
public MsoArrowheadWidth EndArrowWidth { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Drawing;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class LinePropertyEndArrowWidthDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue datos de muestra para el gráfico de líneas
            worksheet.Cells["A1"].PutValue(1);
            worksheet.Cells["A2"].PutValue(2);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(5);
            worksheet.Cells["B3"].PutValue(6);

            // Agregar un gráfico de líneas
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("A1:B3", true);

            // Configure las propiedades de línea para la primera serie
            Series series = chart.NSeries[0];
            series.Border.EndArrowWidth = MsoArrowheadWidth.Wide;
            series.Border.EndType = MsoArrowheadStyle.Arrow;

            // Guarda el libro de trabajo
            workbook.Save("LinePropertyEndArrowWidthDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [MsoArrowheadWidth](../../msoarrowheadwidth/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


