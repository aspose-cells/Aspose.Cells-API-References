---
title: "DataLabels.IsNeverOverlap"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Indica si las etiquetas de datos nunca se superponen al generar una imagen de un gráfico circular. Nota: esta propiedad solo tiene sentido al generar una imagen de un gráfico circular"
type: docs
url: /es/net/aspose.cells.charts/datalabels/isneveroverlap/
---
## DataLabels.IsNeverOverlap property

Indica si las etiquetas de datos nunca se superponen al generar una imagen de gráfico de pastel. Nota: esta propiedad solo tiene sentido cuando se genera una imagen de gráfico de pastel.

```csharp
public bool IsNeverOverlap { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyIsNeverOverlapDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar etiquetas de datos
            Series series = chart.NSeries[0];
            series.DataLabels.ShowValue = true;

            // Obtener etiquetas de datos y establecer la propiedad IsNeverOverlap
            DataLabels dataLabels = series.DataLabels;
            Console.WriteLine("Default IsNeverOverlap value: " + dataLabels.IsNeverOverlap);
            
            // Establecer IsNeverOverlap a verdadero
            dataLabels.IsNeverOverlap = true;
            Console.WriteLine("After setting IsNeverOverlap: " + dataLabels.IsNeverOverlap);

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsIsNeverOverlapDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


