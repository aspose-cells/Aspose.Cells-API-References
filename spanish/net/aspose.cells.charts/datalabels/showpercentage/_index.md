---
title: "DataLabels.ShowPercentage"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad DataLabels. Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. Verdadero muestra el valor del porcentaje. Falso para ocultar"
type: docs
url: /es/net/aspose.cells.charts/datalabels/showpercentage/
---
## DataLabels.ShowPercentage property

Representa el comportamiento de visualización del valor de porcentaje de la etiqueta de datos de un gráfico especificado. True muestra el valor de porcentaje. False lo oculta.

```csharp
public bool ShowPercentage { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class DataLabelsPropertyShowPercentageDemo
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

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar etiquetas de datos y mostrar porcentaje
            DataLabels dataLabels = chart.NSeries[0].DataLabels;
            dataLabels.ShowPercentage = true;
            dataLabels.ShowValue = false;

            // Guarda el libro de trabajo
            workbook.Save("DataLabelsShowPercentageDemo.xlsx");
        }
    }
}
```

### Ver también

* class [DataLabels](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


