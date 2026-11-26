---
title: "Enum ChartSplitType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.ChartSplitType enum. Representa la forma en que se dividen las dos secciones de un gráfico de pastel dentro de pastel o de barra dentro de pastel"
type: docs
url: /es/net/aspose.cells.charts/chartsplittype/
---
## ChartSplitType enumeration

Representa la forma en que se dividen las dos secciones de un gráfico de pastel dentro de pastel o de barra dentro de pastel.

```csharp
public enum ChartSplitType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Position | `0` | Representa los puntos de datos. Los puntos de datos se dividirán entre el pastel y el segundo gráfico colocando la última posición de división de los puntos de datos en el segundo gráfico. |
| Value | `1` | Representa que los puntos de datos se dividirán entre el pastel y el segundo gráfico colocando los puntos de datos con un valor menor que la Posición de División en el segundo gráfico. |
| PercentValue | `2` | Representa los puntos de datos que se dividirán entre el pastel y el segundo gráfico colocando los puntos con un porcentaje menor que el porcentaje de Posición de División en el segundo gráfico. |
| Custom | `3` | Representa que los puntos de datos se dividirán entre el pastel y el segundo gráfico según los valores de División Personalizada. |
| Auto | `4` | Representa los puntos de datos que se dividirán usando el mecanismo predeterminado para este tipo de gráfico. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassChartSplitTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregue datos de muestra para el gráfico
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["A2"].PutValue("A");
                worksheet.Cells["A3"].PutValue("B");
                worksheet.Cells["A4"].PutValue("C");
                worksheet.Cells["A5"].PutValue("D");

                worksheet.Cells["B1"].PutValue("Value");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["B3"].PutValue(20);
                worksheet.Cells["B4"].PutValue(30);
                worksheet.Cells["B5"].PutValue(40);

                // Agregar un gráfico de pastel
                int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
                Chart chart = worksheet.Charts[chartIndex];

                // Establecer rango de datos del gráfico
                chart.NSeries.Add("B2:B5", true);
                chart.NSeries.CategoryData = "A2:A5";

                // Demostrar diferentes valores de ChartSplitType
                chart.NSeries[0].SplitType = ChartSplitType.Position;
                Console.WriteLine($"Current SplitType: {chart.NSeries[0].SplitType}");

                // Cambiar a otro tipo de división
                chart.NSeries[0].SplitType = ChartSplitType.PercentValue;
                Console.WriteLine($"Updated SplitType: {chart.NSeries[0].SplitType}");

                // Guarda el libro de trabajo
                workbook.Save("ChartSplitTypeDemo.xlsx");
                Console.WriteLine("ChartSplitType demonstration completed successfully.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error in ChartSplitType demonstration: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


