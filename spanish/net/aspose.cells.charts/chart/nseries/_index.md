---
title: "Chart.NSeries"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Obtiene una colección SeriesCollection que representa las series de datos en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/nseries/
---
## Chart.NSeries property

Obtiene una colección [`SeriesCollection`](../../seriescollection/) que representa las series de datos en el gráfico.

```csharp
public SeriesCollection NSeries { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyNSeriesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de muestra a las celdas
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["B1"].PutValue("Value");
            for (int i = 2; i <= 10; i++)
            {
                sheet.Cells["A" + i].PutValue("Cat " + (i - 1));
                sheet.Cells["B" + i].PutValue(i * 10);
            }

            // Añade un gráfico
            int chartIndex = sheet.Charts.Add(ChartType.LineWithDataMarkers, 5, 2, 25, 11);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];

            // Establecer la fuente de datos para las series del gráfico usando NSeries
            chart.NSeries.Add("=Sheet1!$A$2:$B$10", true);

            // Establecer título del gráfico
            chart.Title.Text = "NSeries Demo Chart";

            // Guarda el libro de trabajo
            workbook.Save("NSeriesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


