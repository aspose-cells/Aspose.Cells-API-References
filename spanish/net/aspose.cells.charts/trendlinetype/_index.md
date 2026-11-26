---
title: "Enumeración TrendlineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.TrendlineType enum. Representa el tipo de línea de tendencia."
type: docs
url: /es/net/aspose.cells.charts/trendlinetype/
---
## TrendlineType enumeration

Representa el tipo de línea de tendencia.

```csharp
public enum TrendlineType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Exponential | `0` | Exponencial |
| Linear | `1` | Lineal |
| Logarithmic | `2` | Logarítmico |
| MovingAverage | `3` | Media Móvil |
| Polynomial | `4` | Polinómico |
| Power | `5` | Potencia |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class TrendlineTypeDemo
    {
        public static void TrendlineTypeExample()
        {
            // Instanciando un objeto Workbook
            Workbook workbook = new Workbook();
            
            // Añadiendo una nueva hoja de cálculo al objeto Excel
            int sheetIndex = workbook.Worksheets.Add();
            
            // Obteniendo la referencia de la hoja de cálculo recién añadida pasando su índice de hoja
            Worksheet worksheet = workbook.Worksheets[sheetIndex];
            
            // Agregar valores de muestra a celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            
            // Accediendo a la instancia del gráfico recién agregado
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B4"
            chart.NSeries.Add("A1:B4", true);
            
            // Estableciendo la fuente de datos para los datos de categoría de NSeries
            chart.NSeries.CategoryData = "C1:C4";

            // Agregar diferentes tipos de líneas de tendencia al gráfico
            AddTrendline(chart, 0, TrendlineType.Linear, "Linear Trendline");
            AddTrendline(chart, 0, TrendlineType.Exponential, "Exponential Trendline");
            AddTrendline(chart, 0, TrendlineType.Logarithmic, "Logarithmic Trendline");
            AddTrendline(chart, 0, TrendlineType.MovingAverage, "Moving Average Trendline");
            AddTrendline(chart, 0, TrendlineType.Polynomial, "Polynomial Trendline");
            AddTrendline(chart, 0, TrendlineType.Power, "Power Trendline");

            // Guardando el archivo Excel
            workbook.Save("TrendlineTypeExample.xlsx");
        }

        private static void AddTrendline(Chart chart, int seriesIndex, TrendlineType trendlineType, string trendlineName)
        {
            // Agregar una línea de tendencia del tipo especificado a la serie especificada
            int index = chart.NSeries[seriesIndex].TrendLines.Add(trendlineType);
            Trendline trendline = chart.NSeries[seriesIndex].TrendLines[index];
            
            // Estableciendo el nombre personalizado de la línea de tendencia
            trendline.Name = trendlineName;
            
            // Mostrar la ecuación en el gráfico
            trendline.DisplayEquation = true;
            
            // Mostrar el valor R al cuadrado en el gráfico
            trendline.DisplayRSquared = true;
            
            // Establecer el color de la línea de tendencia
            trendline.Color = Color.Red;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


