---
title: "Series.HasHiLoLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Verdadero si el gráfico de líneas tiene líneas de alto/bajo. Se aplica solo a gráficos de líneas"
type: docs
url: /es/net/aspose.cells.charts/series/hashilolines/
---
## Series.HasHiLoLines property

True si el gráfico de líneas tiene líneas alto-bajo. Se aplica solo a gráficos de líneas.

```csharp
public bool HasHiLoLines { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyHasHiLoLinesDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Q3");
            worksheet.Cells["C4"].PutValue("Q4");
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            Series series = chart.NSeries[0];
            series.HasHiLoLines = true;

            workbook.Save("SeriesHasHiLoLinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


