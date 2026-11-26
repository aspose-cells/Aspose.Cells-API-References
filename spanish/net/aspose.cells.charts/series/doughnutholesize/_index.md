---
title: "Series.DoughnutHoleSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Series. Devuelve o establece el tamaño del agujero en un grupo de gráfico de dona. El tamaño del agujero se expresa como un porcentaje del tamaño del gráfico entre el 10 y el 90 por ciento"
type: docs
url: /es/net/aspose.cells.charts/series/doughnutholesize/
---
## Series.DoughnutHoleSize property

Devuelve o establece el tamaño del agujero en un grupo de gráfico de dona. El tamaño del agujero se expresa como un porcentaje del tamaño del gráfico, entre el 10 y el 90 por ciento.

```csharp
public int DoughnutHoleSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyDoughnutHoleSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Agregar un gráfico de anillo
            int chartIndex = worksheet.Charts.Add(ChartType.Doughnut, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad DoughnutHoleSize (porcentaje del radio del gráfico)
            chart.NSeries[0].DoughnutHoleSize = 25;

            // Guarda el libro de trabajo
            workbook.Save("DoughnutHoleSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


