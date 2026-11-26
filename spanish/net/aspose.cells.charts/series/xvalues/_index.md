---
title: "Series.XValues"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Representa los valores X de esta serie de gráfico"
type: docs
url: /es/net/aspose.cells.charts/series/xvalues/
---
## Series.XValues property

Representa los valores X de esta serie de gráfico.

```csharp
public string XValues { get; set; }
```

### Observaciones

Solo para gráficos Scatter y Bubble. Por favor use [`CategoryData`](../../seriescollection/categorydata/) para otros tipos de gráficos, [`CategoryValues`](../categoryvalues/) se usa para obtener los valores de categoría reales de esta serie.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyXValuesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            var workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("X Values");
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["C1"].PutValue("Series 2");
            
            for (int i = 0; i < 5; i++)
            {
                worksheet.Cells[i+1, 0].PutValue(i+1); // X values 1-5
                worksheet.Cells[i+1, 1].PutValue((i+1)*2); // Series 1 values
                worksheet.Cells[i+1, 2].PutValue((i+1)*3); // Series 2 values
            }

            // Agregar un gráfico de dispersión
            int chartIndex = worksheet.Charts.Add(ChartType.Scatter, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar serie con XValues y Values
            int seriesIndex = chart.NSeries.Add("B2:B6", false);
            Series series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property
            series.Name = "Series 1";

            seriesIndex = chart.NSeries.Add("C2:C6", false);
            series = chart.NSeries[seriesIndex];
            series.XValues = "A2:A6"; // Demonstrating XValues property again
            series.Name = "Series 2";

            // Guarda el libro de trabajo
            workbook.Save("SeriesXValuesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


