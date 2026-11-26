---
title: "Series.SecondPlotSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Series. Devuelve o establece el tamaño de la sección secundaria de un gráfico de pastel dentro de otro pastel o de una barra dentro de un pastel como un porcentaje del tamaño del pastel principal. Puede ser un valor de 5 a 200"
type: docs
url: /es/net/aspose.cells.charts/series/secondplotsize/
---
## Series.SecondPlotSize property

Devuelve o establece el tamaño de la sección secundaria de un gráfico de pastel dentro de pastel o de barra dentro de pastel, como un porcentaje del tamaño del pastel principal. Puede ser un valor de 5 a 200.

```csharp
public short SecondPlotSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySecondPlotSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para el gráfico de pastel
            worksheet.Cells["A1"].PutValue("Fruit");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Quantity");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la primera serie
            Series series = chart.NSeries[0];

            // Establecer la propiedad SecondPlotSize (porcentaje del pastel a mostrar en la segunda trama)
            series.SecondPlotSize = 30; // 30% of the pie will be shown in second plot

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertySecondPlotSizeDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


