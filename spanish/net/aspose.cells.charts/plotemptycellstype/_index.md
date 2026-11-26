---
title: "Enumeración PlotEmptyCellsType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.PlotEmptyCellsType enum. Representa todos los tipos de celdas vacías de un gráfico"
type: docs
url: /es/net/aspose.cells.charts/plotemptycellstype/
---
## PlotEmptyCellsType enumeration

Representa todos los tipos de celdas vacías del trazado de un gráfico.

```csharp
public enum PlotEmptyCellsType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| NotPlotted | `0` | No trazado (dejar hueco) |
| Zero | `1` | Cero |
| Interpolated | `2` | Interpolado |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class PlotEmptyCellsTypeDemo
    {
        public static void PlotEmptyCellsTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(null); // Empty cell
            worksheet.Cells["A5"].PutValue("D");
            worksheet.Cells["B5"].PutValue(40);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 7, 1, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer el rango de datos para el gráfico
            chart.SetChartDataRange("A1:B5", true);

            // Establecer el título del gráfico
            chart.Title.Text = "Plot Empty Cells Example";

            // Establece cómo trazar celdas vacías
            chart.PlotEmptyCellsType = PlotEmptyCellsType.Interpolated;

            // Guarda el libro de trabajo
            workbook.Save("PlotEmptyCellsTypeExample.xlsx");

            Console.WriteLine("Workbook saved successfully.");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


