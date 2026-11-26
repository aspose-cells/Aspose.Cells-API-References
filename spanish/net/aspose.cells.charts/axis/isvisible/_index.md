---
title: "Axis.IsVisible"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Axis. Representa si el eje es visible"
type: docs
url: /es/net/aspose.cells.charts/axis/isvisible/
---
## Axis.IsVisible property

Representa si el eje es visible.

```csharp
public bool IsVisible { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class AxisPropertyIsVisibleDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Agregar una serie de eje secundario
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries[1].PlotOnSecondAxis = true;

            // Demostrar la propiedad IsVisible
            Console.WriteLine("Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);
            
            // Ocultar el eje secundario
            chart.SecondValueAxis.IsVisible = false;
            Console.WriteLine("After setting to false - Secondary Value Axis Visible: " + chart.SecondValueAxis.IsVisible);

            // Guarda el libro de trabajo
            workbook.Save("AxisIsVisibleDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


