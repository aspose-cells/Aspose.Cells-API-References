---
title: "SeriesLayoutProperties.IsIntervalLeftClosed"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesLayoutProperties. Indica si el intervalo está cerrado en el lado izquierdo"
type: docs
url: /es/net/aspose.cells.charts/serieslayoutproperties/isintervalleftclosed/
---
## SeriesLayoutProperties.IsIntervalLeftClosed property

Indica si el intervalo está cerrado en el lado izquierdo.

```csharp
public bool IsIntervalLeftClosed { get; set; }
```

### Observaciones

Solo para el gráfico ParetoLine.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyIsIntervalLeftClosedDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["B1"].PutValue(15);
            worksheet.Cells["B2"].PutValue(25);
            worksheet.Cells["B3"].PutValue(35);

            // Crear gráfico
            int chartIndex = worksheet.Charts.Add(Aspose.Cells.Charts.ChartType.Column, 5, 0, 15, 5);
            Aspose.Cells.Charts.Chart chart = worksheet.Charts[chartIndex];
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Aspose.Cells.Charts.Series series = chart.NSeries[seriesIndex];

            // Establecer la propiedad IsIntervalLeftClosed
            series.LayoutProperties.IsIntervalLeftClosed = true;

            // Guardar el libro de trabajo
            workbook.Save("SeriesLayoutPropertiesIsIntervalLeftClosedDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


