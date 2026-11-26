---
title: "Series.SplitType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Devuelve o establece un valor que indica cómo determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel."
type: docs
url: /es/net/aspose.cells.charts/series/splittype/
---
## Series.SplitType property

Devuelve o establece un valor que indica cómo determinar qué puntos de datos están en el segundo pastel o barra en un gráfico de pastel dentro de pastel o barra dentro de pastel.

```csharp
public ChartSplitType SplitType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertySplitTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo para el gráfico
            sheet.Cells["A1"].PutValue("Category");
            sheet.Cells["A2"].PutValue("A");
            sheet.Cells["A3"].PutValue("B");
            sheet.Cells["A4"].PutValue("C");
            sheet.Cells["B1"].PutValue("Value");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Agregar un gráfico de pastel
            int chartIndex = sheet.Charts.Add(ChartType.Pie, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer el tipo de división para la primera serie
            chart.NSeries[0].SplitType = ChartSplitType.Position;

            // Guarda el libro de trabajo
            workbook.Save("SeriesPropertySplitTypeDemo_out.xlsx");
        }
    }
}
```

### Ver también

* enum [ChartSplitType](../../chartsplittype/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


