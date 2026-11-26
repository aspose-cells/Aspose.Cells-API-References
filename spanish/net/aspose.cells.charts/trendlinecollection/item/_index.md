---
title: "TrendlineCollection.Item"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad TrendlineCollection. Obtiene un objeto Trendline por su índice"
type: docs
url: /es/net/aspose.cells.charts/trendlinecollection/item/
---
## TrendlineCollection indexer

Obtiene un objeto [`Trendline`](../../trendline/) por su índice.

```csharp
public Trendline this[int index] { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class TrendlineCollectionPropertyItemDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(1);
            sheet.Cells["A2"].PutValue(2);
            sheet.Cells["A3"].PutValue(3);
            sheet.Cells["B1"].PutValue(4);
            sheet.Cells["B2"].PutValue(5);
            sheet.Cells["B3"].PutValue(6);

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer origen de datos del Chart
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries[0].Values = "B1:B3";

            // Añadir una línea de tendencia
            int trendlineIndex = chart.NSeries[0].TrendLines.Add(TrendlineType.Linear);
            Trendline trendline = chart.NSeries[0].TrendLines[trendlineIndex];

            // Demostrar el uso de la propiedad Item
            Trendline firstTrendline = chart.NSeries[0].TrendLines[0];
            Console.WriteLine("Trendline Type: " + firstTrendline.Type);
        }
    }
}
```

### Ver también

* class [Trendline](../../trendline/)
* class [TrendlineCollection](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


