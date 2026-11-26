---
title: "ChartShape.Chart"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ChartShape. Devuelve un objeto Chart que representa el gráfico contenido en el objeto"
type: docs
url: /es/net/aspose.cells.drawing/chartshape/chart/
---
## ChartShape.Chart property

Devuelve un objeto Chart que representa el gráfico contenido en el objeto.

```csharp
public Chart Chart { get; }
```

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using Aspose.Cells.Drawing;
    using System;

    public class ChartShapePropertyChartDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Fruits");
            worksheet.Cells["A3"].PutValue("Vegetables");
            worksheet.Cells["A4"].PutValue("Grains");
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(50);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(20);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la instancia de ChartShape
            ChartShape chartShape = (ChartShape)chart.ChartObject;

            // Acceder a la propiedad Chart (solo lectura)
            Chart accessedChart = chartShape.Chart;

            // Mostrar propiedades del gráfico
            Console.WriteLine("Chart Name: " + accessedChart.Name);
            Console.WriteLine("Chart Type: " + accessedChart.Type);
            Console.WriteLine("Show Legend: " + accessedChart.ShowLegend);

            // Modificar las propiedades del gráfico a través del objeto Chart
            accessedChart.Name = "Sales Chart";
            accessedChart.ShowLegend = false;
            accessedChart.Title.Text = "Product Sales Distribution";

            // Cambiar el tipo de gráfico
            accessedChart.Type = ChartType.Pie;

            // Guardar el resultado
            workbook.Save("ChartShapePropertyChartDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Chart](../../../aspose.cells.charts/chart/)
* class [ChartShape](../)
* namespace [Aspose.Cells.Drawing](../../../aspose.cells.drawing/)
* assembly [Aspose.Cells](../../../)


