---
title: "ChartArea.WidthRatioToChart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartArea. Obtiene o establece el desplazamiento horizontal desde la columna de su esquina inferior derecha en unidades de razón del área del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartarea/widthratiotochart/
---
## ChartArea.WidthRatioToChart property

Obtiene o establece el desplazamiento horizontal desde la columna de su esquina inferior derecha, en unidades de proporción del área del gráfico.

```csharp
public override double WidthRatioToChart { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartAreaPropertyWidthRatioToChartDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de columnas
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 10);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Calcular gráfico
            chart.Calculate();

            // Demuestre la propiedad WidthRatioToChart
            Console.WriteLine("Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
            
            // Modifique la razón y muestre el cambio
            chart.ChartArea.WidthRatioToChart = 0.8;
            Console.WriteLine("Modified Chart Area Width Ratio: " + chart.ChartArea.WidthRatioToChart);
        }
    }
}
```

### Ver también

* class [ChartArea](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


