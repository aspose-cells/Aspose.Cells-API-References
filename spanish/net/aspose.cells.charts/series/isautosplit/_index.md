---
title: "Series.IsAutoSplit"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Indica si el valor del umbral es automático"
type: docs
url: /es/net/aspose.cells.charts/series/isautosplit/
---
## Series.IsAutoSplit property

Indica si el valor del umbral es automático.

```csharp
public bool IsAutoSplit { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyIsAutoSplitDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregue datos de muestra para el gráfico
            worksheet.Cells["A1"].PutValue("Category");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["A3"].PutValue("Orange");
            worksheet.Cells["A4"].PutValue("Banana");
            worksheet.Cells["A5"].PutValue("Grape");
            
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);
            worksheet.Cells["B5"].PutValue(40);

            // Agregar un gráfico de pastel
            int chartIndex = worksheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B5", true);
            chart.NSeries.CategoryData = "A2:A5";

            // Acceder a la primera serie y demostrar la propiedad IsAutoSplit
            Series series = chart.NSeries[0];
            bool isAutoSplit = series.IsAutoSplit; // Get the value instead of setting it
            series.SplitValue = 25; // Split at value 25

            Console.WriteLine($"IsAutoSplit value: {isAutoSplit}");

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyIsAutoSplitDemo_out.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


