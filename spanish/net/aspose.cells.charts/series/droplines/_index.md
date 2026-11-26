---
title: "Series.DropLines"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Devuelve un objeto Line que representa las líneas de caída para una serie en el gráfico de líneas o de áreas. Se aplica solo a gráficos de líneas o de áreas"
type: docs
url: /es/net/aspose.cells.charts/series/droplines/
---
## Series.DropLines property

Devuelve un objeto [`Line`](../../../aspose.cells.drawing/line/) que representa las líneas de caída para una serie en el gráfico de líneas o de áreas. Se aplica solo a gráficos de líneas o de áreas.

```csharp
public Line DropLines { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class SeriesPropertyDropLinesDemo
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

            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(120);
            worksheet.Cells["B3"].PutValue(150);
            worksheet.Cells["B4"].PutValue(180);
            worksheet.Cells["B5"].PutValue(210);

            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(90);
            worksheet.Cells["C3"].PutValue(130);
            worksheet.Cells["C4"].PutValue(160);
            worksheet.Cells["C5"].PutValue(190);

            // Agregar un gráfico de líneas
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 6, 0, 20, 10);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.Add("C2:C5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Habilitar líneas de caída para el gráfico
            chart.NSeries[0].HasDropLines = true;
            chart.NSeries[1].HasDropLines = true;

            // Acceder a las líneas de caída de la primera serie
            Line dropLines = chart.NSeries[0].DropLines;

            // Mostrar las propiedades actuales de las líneas de caída
            Console.WriteLine("Drop line color: " + dropLines.Color);
            Console.WriteLine("Drop line style: " + dropLines.Style);
            Console.WriteLine("Drop line weight: " + dropLines.Weight);

            // Modificar las propiedades de las líneas de caída
            dropLines.Color = System.Drawing.Color.Red;
            dropLines.Style = LineType.Solid;
            dropLines.Weight = WeightType.MediumLine;
            dropLines.DashType = MsoLineDashStyle.Solid;
            dropLines.IsVisible = true;

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyDropLinesDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


