---
title: "Series.YErrorBar"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Series. Representa la barra de error en dirección Y de la serie"
type: docs
url: /es/net/aspose.cells.charts/series/yerrorbar/
---
## Series.YErrorBar property

Representa la barra de error en dirección Y de la serie.

```csharp
public ErrorBar YErrorBar { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesPropertyYErrorBarDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue("X");
            sheet.Cells["A2"].PutValue(1);
            sheet.Cells["A3"].PutValue(2);
            sheet.Cells["A4"].PutValue(3);
            sheet.Cells["B1"].PutValue("Y");
            sheet.Cells["B2"].PutValue(10);
            sheet.Cells["B3"].PutValue(20);
            sheet.Cells["B4"].PutValue(30);

            // Crear gráfico
            int chartIndex = sheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = sheet.Charts[chartIndex];
            chart.NSeries.Add("B2:B4", true);
            chart.NSeries.CategoryData = "A2:A4";

            // Establecer propiedades de YErrorBar
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.Type = ErrorBarType.Percent;
            errorBar.Amount = 5;
            errorBar.DisplayType = ErrorBarDisplayType.Both;

            // Guarda el libro de trabajo
            workbook.Save("YErrorBarDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ErrorBar](../../errorbar/)
* class [Series](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


