---
title: "Series.Area"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad de Series. Representa el área de fondo del objeto Series"
type: docs
url: /es/net/aspose.cells.charts/series/area/
---
## Series.Area property

Representa el área de fondo del objeto Series.

```csharp
public Area Area { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class SeriesPropertyAreaDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("A");
            worksheet.Cells["A3"].PutValue("B");
            worksheet.Cells["A4"].PutValue("C");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Acceder a la primera serie y establecer la textura del área
            Series series = chart.NSeries[0];
            series.Area.FillFormat.Texture = TextureType.Stationery;

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyAreaDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [Area](../../../aspose.cells.drawing/area/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


