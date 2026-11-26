---
title: "Chart.FilteredNSeries"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Chart propiedad. Obtiene una colección SeriesCollection que representa las series de datos que están filtradas en el gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/filterednseries/
---
## Chart.FilteredNSeries property

Obtiene una colección [`SeriesCollection`](../../seriescollection/) que representa las series de datos que están filtradas en el gráfico.

```csharp
public SeriesCollection FilteredNSeries { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertyFilteredNSeriesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Series 1");
            worksheet.Cells["A3"].PutValue("Series 2");
            worksheet.Cells["A4"].PutValue("Series 3");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico y establecer algunas series como filtradas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Filtrar algunas series (ocultar Series 2)
            chart.NSeries[1].IsFiltered = true;

            // Acceder a la colección de series filtradas
            Aspose.Cells.Charts.SeriesCollection filteredSeries = chart.FilteredNSeries;
            Console.WriteLine("Filtered Series Count: " + filteredSeries.Count.ToString());

            // Guarda el libro de trabajo
            workbook.Save("FilteredNSeriesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesCollection](../../seriescollection/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


