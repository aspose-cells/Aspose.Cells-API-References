---
title: "Series.XErrorBar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Representa la barra de error en dirección X de la serie"
type: docs
url: /es/net/aspose.cells.charts/series/xerrorbar/
---
## Series.XErrorBar property

Representa la barra de error en dirección X de la serie.

```csharp
public ErrorBar XErrorBar { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXErrorBarDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Y Values");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregue series usando los datos
            SeriesCollection seriesCollection = chart.NSeries;
            seriesCollection.Add("B2:B4", true);
            Series series = seriesCollection[0];
            series.XValues = "A2:A4";

            // Configure las propiedades de XErrorBar
            series.XErrorBar.DisplayType = ErrorBarDisplayType.Plus;
            series.XErrorBar.Amount = 0.5;
            series.XErrorBar.Type = ErrorBarType.FixedValue;

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyXErrorBarDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


