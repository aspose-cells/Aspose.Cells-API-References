---
title: "Series.IsColorVaried"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Representa si el color de los puntos es variado. El gráfico debe contener solo una serie o ser un gráfico circular"
type: docs
url: /es/net/aspose.cells.charts/series/iscolorvaried/
---
## Series.IsColorVaried property

Representa si el color de los puntos varía. El gráfico debe contener solo una serie o ser un gráfico de pastel.

```csharp
public bool IsColorVaried { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsColorVariedDemo
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
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad IsColorVaried para la primera serie
            chart.NSeries[0].IsColorVaried = true;

            // Guarda el libro de trabajo
            workbook.Save("output.xlsx");

            // Verificar la propiedad
            Console.WriteLine("IsColorVaried: " + chart.NSeries[0].IsColorVaried);
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


