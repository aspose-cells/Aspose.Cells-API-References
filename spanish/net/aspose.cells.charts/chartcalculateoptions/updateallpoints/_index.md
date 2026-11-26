---
title: "ChartCalculateOptions.UpdateAllPoints"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartCalculateOptions. Indica si se actualizan todos los puntos de datos al realizar el cálculo del gráfico. Predeterminado False. Cuando desea obtener el valor de cada punto de datos en el gráfico, configúrelo específicamente en verdadero. Si este parámetro se establece en True, pueden generarse nuevos puntos de datos cuando se calcula el gráfico. Esto podría hacer que el archivo de Excel sea más grande"
type: docs
url: /es/net/aspose.cells.charts/chartcalculateoptions/updateallpoints/
---
## ChartCalculateOptions.UpdateAllPoints property

Indica si se actualizan todos los puntos de datos al realizar el cálculo del gráfico. Predeterminado: False. Cuando desea obtener el valor de cada punto de datos en el gráfico específicamente, configúrelo en true. Si este parámetro se establece en True, pueden generarse nuevos puntos de datos cuando se calcula el gráfico. Esto podría hacer que el archivo de Excel sea más grande.

```csharp
public bool UpdateAllPoints { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartCalculateOptionsPropertyUpdateAllPointsDemo
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
            
            worksheet.Cells["B1"].PutValue("Series1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series2");
            worksheet.Cells["C2"].PutValue(400);
            worksheet.Cells["C3"].PutValue(500);
            worksheet.Cells["C4"].PutValue(600);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";
            
            // Habilitar etiquetas de datos
            foreach (Aspose.Cells.Charts.Series series in chart.NSeries)
            {
                series.DataLabels.ShowValue = true;
            }

            // Calcular el gráfico con la opción UpdateAllPoints
            chart.Calculate(new Aspose.Cells.Charts.ChartCalculateOptions() { UpdateAllPoints = true });

            // Salida de algunos valores de etiquetas de datos para demostrar el resultado
            Console.WriteLine("Series1 Point1 Label: " + chart.NSeries[0].Points[0].DataLabels.Text);
            Console.WriteLine("Series2 Point2 Label: " + chart.NSeries[1].Points[1].DataLabels.Text);
        }
    }
}
```

### Ver también

* class [ChartCalculateOptions](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


