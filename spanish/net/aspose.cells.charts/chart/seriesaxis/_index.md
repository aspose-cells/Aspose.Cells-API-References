---
title: "Chart.SeriesAxis"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad del gráfico. Obtiene el eje de series del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/seriesaxis/
---
## Chart.SeriesAxis property

Obtiene el eje de series del gráfico.

```csharp
public Axis SeriesAxis { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySeriesAxisDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Series");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["B1"].PutValue("Product A");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            worksheet.Cells["C1"].PutValue("Product B");
            worksheet.Cells["C2"].PutValue(150);
            worksheet.Cells["C3"].PutValue(250);
            worksheet.Cells["C4"].PutValue(350);

            // Agregar un gráfico de columnas agrupadas en 3D
            int chartIndex = worksheet.Charts.Add(ChartType.Column3DClustered, 5, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B1:C4", true);

            // Acceder y configurar el SeriesAxis
            Axis seriesAxis = chart.SeriesAxis;
            seriesAxis.Title.Text = "Product Series";
            seriesAxis.Title.Font.Size = 12;
            seriesAxis.Title.Font.IsBold = true;
            seriesAxis.MajorTickMark = TickMarkType.Cross;
            seriesAxis.MinorTickMark = TickMarkType.Outside;

            // Guarda el libro de trabajo
            workbook.Save("ChartPropertySeriesAxisDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


