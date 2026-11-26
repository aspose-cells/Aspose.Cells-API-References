---
title: "Series.LegendEntry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Obtiene la entrada de leyenda según esta serie"
type: docs
url: /es/net/aspose.cells.charts/series/legendentry/
---
## Series.LegendEntry property

Obtiene la entrada de leyenda correspondiente a esta serie.

```csharp
public LegendEntry LegendEntry { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyLegendEntryDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Obtener la primera serie
            Series series = chart.NSeries[0];

            // Demostrar la funcionalidad de LegendEntry
            Console.WriteLine("LegendEntry.IsDeleted before: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = true;
            Console.WriteLine("LegendEntry.IsDeleted after setting to true: " + series.LegendEntry.IsDeleted);
            series.LegendEntry.IsDeleted = false;
            Console.WriteLine("LegendEntry.IsDeleted after setting to false: " + series.LegendEntry.IsDeleted);

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertyLegendEntryDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [LegendEntry](../../legendentry/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


