---
title: "Enum PlotDataByType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.PlotDataByType enum. Representa el tipo de trazado de datos por fila o columna"
type: docs
url: /es/net/aspose.cells.charts/plotdatabytype/
---
## PlotDataByType enumeration

Representa el tipo de trazado de datos por fila o columna.

```csharp
public enum PlotDataByType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Row | `0` | Ordenado por fila. |
| Column | `1` | Por columna. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ChartsClassPlotDataByTypeDemo
    {
        public static void Run()
        {
            // Cree un nuevo libro de trabajo para la demostración
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            try
            {
                // Agregar datos de ejemplo a la hoja de cálculo
                worksheet.Cells["A1"].PutValue("Category");
                worksheet.Cells["B1"].PutValue("Value1");
                worksheet.Cells["C1"].PutValue("Value2");
                worksheet.Cells["A2"].PutValue("Row1");
                worksheet.Cells["B2"].PutValue(10);
                worksheet.Cells["C2"].PutValue(20);
                worksheet.Cells["A3"].PutValue("Row2");
                worksheet.Cells["B3"].PutValue(30);
                worksheet.Cells["C3"].PutValue(40);

                // Agregar un gráfico a la hoja de cálculo
                int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 25, 10);
                Chart chart = worksheet.Charts[chartIndex];

                // Establecer el rango de datos del gráfico
                chart.NSeries.Add("B2:C3", true);

                // Demostrar el uso de los valores del enum PlotDataByType
                PlotDataByType plotType = PlotDataByType.Row;
                Console.WriteLine($"Chart is currently plotting data by: {plotType}");

                // Cambiar a trazar por columna
                plotType = PlotDataByType.Column;
                Console.WriteLine($"Chart is now plotting data by: {plotType}");

                // Guarda el libro de trabajo
                workbook.Save("PlotDataByTypeDemo.xlsx");
                Console.WriteLine("Workbook saved successfully with PlotDataByType demonstration.");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error working with PlotDataByType: {ex.Message}");
            }
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


