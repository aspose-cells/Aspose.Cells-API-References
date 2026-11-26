---
title: "Series.HiLoLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Devuelve un objeto HiLoLines que representa las líneas alto/bajo para una serie en un gráfico de líneas. Se aplica solo a gráficos de líneas"
type: docs
url: /es/net/aspose.cells.charts/series/hilolines/
---
## Series.HiLoLines property

Devuelve un objeto HiLoLines que representa las líneas alto-bajo para una serie en un gráfico de líneas. Se aplica solo a gráficos de líneas.

```csharp
public Line HiLoLines { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyHiLoLinesDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Q1");
            worksheet.Cells["A3"].PutValue("Q2");
            worksheet.Cells["A4"].PutValue("Q3");
            worksheet.Cells["A5"].PutValue("Q4");

            worksheet.Cells["B1"].PutValue("High");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(90);
            worksheet.Cells["B4"].PutValue(150);
            worksheet.Cells["B5"].PutValue(110);

            worksheet.Cells["C1"].PutValue("Low");
            worksheet.Cells["C2"].PutValue(80);
            worksheet.Cells["C3"].PutValue(60);
            worksheet.Cells["C4"].PutValue(100);
            worksheet.Cells["C5"].PutValue(70);

            // Agregar un gráfico de líneas
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B1:B5", true);
            chart.NSeries.Add("C1:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Habilitar HiLoLines para la primera serie
            Series series = chart.NSeries[0];
            series.HasHiLoLines = true;

            // Acceder y modificar las propiedades de HiLoLines
            Line hiLoLines = series.HiLoLines;
            Console.WriteLine("HiLoLines visibility: " + hiLoLines.IsVisible);

            // Personalizar la apariencia de HiLoLines
            hiLoLines.Color = System.Drawing.Color.Red;
            hiLoLines.Weight = WeightType.MediumLine;
            hiLoLines.DashType = MsoLineDashStyle.DashDot;
            hiLoLines.IsVisible = true;

            // Guardar el resultado
            workbook.Save("SeriesPropertyHiLoLinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


