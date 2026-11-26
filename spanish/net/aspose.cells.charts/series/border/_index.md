---
title: "Series.Border"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Representa el borde de un objeto Series"
type: docs
url: /es/net/aspose.cells.charts/series/border/
---
## Series.Border property

Representa el borde de un objeto Series.

```csharp
public Line Border { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyBorderDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Year");
            worksheet.Cells["A2"].PutValue("2020");
            worksheet.Cells["A3"].PutValue("2021");
            worksheet.Cells["A4"].PutValue("2022");
            
            worksheet.Cells["B1"].PutValue("Sales");
            worksheet.Cells["B2"].PutValue(5000);
            worksheet.Cells["B3"].PutValue(7000);
            worksheet.Cells["B4"].PutValue(9000);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar datos de la serie
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la primera serie
            Series series = chart.NSeries[0];
            series.Name = "Sales Data";

            // Personalizar las propiedades del borde
            series.Border.Color = System.Drawing.Color.Blue;
            series.Border.Weight = WeightType.MediumLine;
            series.Border.DashType = MsoLineDashStyle.Solid;
            series.Border.IsVisible = true;

            // Guarda el libro de trabajo
            workbook.Save("SeriesBorderDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Line](../../../aspose.cells.drawing/line/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


