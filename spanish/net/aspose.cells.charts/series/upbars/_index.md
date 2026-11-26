---
title: "Series.UpBars"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Devuelve un objeto DropBars que representa las barras superiores en un gráfico de líneas. Se aplica solo a gráficos de líneas"
type: docs
url: /es/net/aspose.cells.charts/series/upbars/
---
## Series.UpBars property

Devuelve un objeto DropBars que representa las barras ascendentes en un gráfico de líneas. Se aplica solo a gráficos de líneas.

```csharp
public DropBars UpBars { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyUpBarsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Datos de ejemplo para un gráfico de líneas con barras arriba/abajo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Habilitar y personalizar las barras superiores
            chart.NSeries[0].HasUpDownBars = true;
            DropBars upBars = chart.NSeries[0].UpBars;
            upBars.Area.ForegroundColor = Color.LightGreen;
            upBars.Border.Color = Color.Green;

            workbook.Save("UpBarsExample.xlsx");
        }
    }
}
```

### Ver también

* class [DropBars](../../dropbars/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


