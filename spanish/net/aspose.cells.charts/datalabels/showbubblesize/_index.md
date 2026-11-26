---
title: "DataLabels.ShowBubbleSize"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False oculta el valor de porcentaje"
type: docs
url: /es/net/aspose.cells.charts/datalabels/showbubblesize/
---
## DataLabels.ShowBubbleSize property

Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False oculta el valor de porcentaje.

```csharp
public bool ShowBubbleSize { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowBubbleSizeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico de burbujas
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["C1"].PutValue("Size");
            worksheet.Cells["C2"].PutValue(5);
            worksheet.Cells["C3"].PutValue(10);
            worksheet.Cells["C4"].PutValue(15);

            // Agregar un gráfico de burbujas
            int chartIndex = worksheet.Charts.Add(ChartType.Bubble, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar series al gráfico
            int seriesIndex = chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Establecer tamaños de burbujas para la serie
            Series series = chart.NSeries[seriesIndex];
            series.BubbleSizes = "C2:C4";

            // Acceder a los DataLabels de la serie
            DataLabels dataLabels = series.DataLabels;

            // Demostrar la propiedad ShowBubbleSize
            dataLabels.ShowBubbleSize = true; // Show bubble size in data labels
            dataLabels.ShowValue = true;      // Also show values for clarity

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsShowBubbleSizeDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


