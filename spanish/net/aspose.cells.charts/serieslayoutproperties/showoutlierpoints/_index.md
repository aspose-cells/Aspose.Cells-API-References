---
title: "SeriesLayoutProperties.ShowOutlierPoints"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SeriesLayoutProperties. Indica si se muestran los puntos de datos atípicos"
type: docs
url: /es/net/aspose.cells.charts/serieslayoutproperties/showoutlierpoints/
---
## SeriesLayoutProperties.ShowOutlierPoints property

Indica si se muestran los puntos de datos atípicos.

```csharp
public bool ShowOutlierPoints { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowOutlierPointsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(10);
            worksheet.Cells["A2"].PutValue(20);
            worksheet.Cells["A3"].PutValue(30);
            worksheet.Cells["A4"].PutValue(200); // Outlier value
            worksheet.Cells["B1"].PutValue("Q1");
            worksheet.Cells["B2"].PutValue("Q2");
            worksheet.Cells["B3"].PutValue("Q3");
            worksheet.Cells["B4"].PutValue("Q4");

            // Cree un gráfico de columnas (que admite puntos atípicos)
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie
            chart.NSeries.Add("A1:A4", true);
            chart.NSeries.CategoryData = "B1:B4";
            
            // Configure las propiedades de diseño de series
            Series series = chart.NSeries[0];
            SeriesLayoutProperties layoutProperties = series.LayoutProperties;
            
            // Demuestre la propiedad ShowOutlierPoints
            layoutProperties.ShowOutlierPoints = true;
            layoutProperties.ShowInnerPoints = true;
            layoutProperties.ShowMeanMarker = true;

            workbook.Save("ChartWithOutliers.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


