---
title: "SeriesLayoutProperties.ShowMeanMarker"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesLayoutProperties. Indica si se muestran los marcadores que denotan la media"
type: docs
url: /es/net/aspose.cells.charts/serieslayoutproperties/showmeanmarker/
---
## SeriesLayoutProperties.ShowMeanMarker property

Indica si se muestran los marcadores que denotan la media.

```csharp
public bool ShowMeanMarker { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowMeanMarkerDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(40);

            // Crear gráfico (usando el tipo de gráfico de columna que admite marcadores de media)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie
            chart.NSeries.Add("A1:A4", true);
            Series series = chart.NSeries[0];

            // Configurar propiedades de diseño con ShowMeanMarker
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            layoutProperties.ShowMeanMarker = true;
            layoutProperties.ShowMeanLine = true;

            // Guardar salida
            workbook.Save("ColumnChartWithMeanMarker.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


