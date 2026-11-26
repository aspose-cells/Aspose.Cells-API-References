---
title: "Trendline.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Trendline. Devuelve el tipo de línea de tendencia"
type: docs
url: /es/net/aspose.cells.charts/trendline/type/
---
## Trendline.Type property

Devuelve el tipo de línea de tendencia.

```csharp
public TrendlineType Type { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlinePropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["A5"].PutValue(4);
            
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(2);
            sheet.Cells["B3"].PutValue(4);
            sheet.Cells["B4"].PutValue(8);
            sheet.Cells["B5"].PutValue(16);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Agregar serie
            chart.NSeries.Add("A2:A5", true);
            chart.NSeries[0].XValues = "B2:B5";

            // Agregar línea de tendencia exponencial
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Exponential);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];
            
            // Demostrar el uso de la propiedad Type
            Console.WriteLine("Trendline type: " + trendline.Type);
            
            // Guarda el libro de trabajo
            workbook.Save("TrendlinePropertyTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [TrendlineType](../../trendlinetype/)
* class [Trendline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


