---
title: "Series.Overlap"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Especifica cómo se posicionan las barras y columnas. Puede ser un valor entre 100 y 100. Se aplica solo a gráficos de barras 2D y columnas 2D"
type: docs
url: /es/net/aspose.cells.charts/series/overlap/
---
## Series.Overlap property

Especifica cómo se posicionan las barras y columnas. Puede ser un valor entre -100 y 100. Se aplica solo a gráficos de barras 2D y gráficos de columnas 2D.

```csharp
public short Overlap { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyOverlapDemo
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
            sheet.Cells["B1"].PutValue("Series1");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);
            sheet.Cells["C1"].PutValue("Series2");
            sheet.Cells["C2"].PutValue(15);
            sheet.Cells["C3"].PutValue(25);
            sheet.Cells["C4"].PutValue(35);

            // Agregue un gráfico de columnas agrupadas
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Aspose.Cells.Charts.Chart chart = sheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer la propiedad overlap para la primera serie
            chart.NSeries[0].Overlap = -40;

            // Guarda el libro de trabajo
            workbook.Save("SeriesOverlapDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


