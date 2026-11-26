---
title: "Line.Style"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Line. Representa el estilo de la línea"
type: docs
url: /es/net/aspose.cells.drawing/line/style/
---
## Line.Style property

Representa el estilo de la línea.

```csharp
public LineType Style { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class LinePropertyStyleDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Crea un gráfico de ejemplo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            
            chart.NSeries.Add("B2:B3", true);
            chart.NSeries.CategoryData = "A2:A3";
            
            // Obtenga la primera serie y su primer punto
            Series series = chart.NSeries[0];
            ChartPoint point = series.Points[0];
            
            // Establecer propiedades de línea
            point.Border.Color = Color.Red;
            point.Border.Style = LineType.Solid;
            
            // Verifique que el estilo se haya establecido
            Console.WriteLine("Border Style: " + point.Border.Style);
            
            workbook.Save("output.xlsx");
        }
    }
}
```

### Ver también

* enum [LineType](../../linetype/)
* class [Line](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


