---
title: "Chart.SecondValueAxis"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Chart. Obtiene el segundo eje Y del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chart/secondvalueaxis/
---
## Chart.SecondValueAxis property

Obtiene el segundo eje Y del gráfico.

```csharp
public Axis SecondValueAxis { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ChartPropertySecondValueAxisDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["B3"].PutValue(200);
            worksheet.Cells["B4"].PutValue(300);
            
            worksheet.Cells["C1"].PutValue("Series 2");
            worksheet.Cells["C2"].PutValue(5000);
            worksheet.Cells["C3"].PutValue(3000);
            worksheet.Cells["C4"].PutValue(1000);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.Add("C2:C4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Habilitar el eje de valores secundario para la segunda serie
            chart.NSeries[1].PlotOnSecondAxis = true;

            // Personalizar el eje de valores secundario
            Axis secondValueAxis = chart.SecondValueAxis;
            secondValueAxis.Title.Text = "Secondary Axis";
            secondValueAxis.MinValue = 0;
            secondValueAxis.MaxValue = 6000;
            secondValueAxis.MajorUnit = 1000;

            // Guarda el libro de trabajo
            workbook.Save("SecondValueAxisDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Axis](../../axis/)
* class [Chart](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


