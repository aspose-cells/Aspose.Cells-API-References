---
title: "SeriesLayoutProperties.ShowInnerPoints"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "SeriesLayoutProperties propiedad. Indica si se deben mostrar los puntos de datos no atípicos"
type: docs
url: /es/net/aspose.cells.charts/serieslayoutproperties/showinnerpoints/
---
## SeriesLayoutProperties.ShowInnerPoints property

Indica si se muestran puntos de datos que no son valores atípicos.

```csharp
public bool ShowInnerPoints { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SeriesLayoutPropertiesPropertyShowInnerPointsDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de muestra para el gráfico de caja y bigotes
            worksheet.Cells["A1"].PutValue("Series 1");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(40);
            worksheet.Cells["A4"].PutValue(15);
            worksheet.Cells["A5"].PutValue(20);
            worksheet.Cells["A6"].PutValue(25);
            worksheet.Cells["A7"].PutValue(30);
            worksheet.Cells["A8"].PutValue(35);
            worksheet.Cells["A9"].PutValue(40);
            worksheet.Cells["A10"].PutValue(45);
            worksheet.Cells["A11"].PutValue(50);

            // Agregar un gráfico de caja y bigotes
            int chartIndex = worksheet.Charts.Add(ChartType.BoxWhisker, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series al gráfico
            chart.NSeries.Add("A2:A11", true);
            Series series = chart.NSeries[0];

            // Establecer propiedades de diseño de series
            SeriesLayoutProperties layout = series.LayoutProperties;
            layout.ShowInnerPoints = true; // Demonstrate ShowInnerPoints property
            layout.ShowOutlierPoints = true;
            layout.ShowMeanMarker = true;

            // Calcular gráfico
            chart.Calculate();

            // Guarda el libro de trabajo
            workbook.Save("BoxWhiskerChart_ShowInnerPoints.xlsx");
        }
    }
}
```

### Ver también

* class [SeriesLayoutProperties](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


