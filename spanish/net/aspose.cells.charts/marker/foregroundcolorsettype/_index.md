---
title: "Marker.ForegroundColorSetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Marker. Obtiene o establece el tipo de conjunto de color de primer plano del marcador"
type: docs
url: /es/net/aspose.cells.charts/marker/foregroundcolorsettype/
---
## Marker.ForegroundColorSetType property

Obtiene o establece el tipo de conjunto de color de primer plano del marcador.

```csharp
public FormattingType ForegroundColorSetType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyForegroundColorSetTypeDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Agregar gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie
            chart.NSeries.Add("A1:B3", true);
            
            // Configurar el marcador de la serie
            Series series = chart.NSeries[0];
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.ForegroundColorSetType = FormattingType.Automatic;
            series.Marker.ForegroundColor = System.Drawing.Color.Black;

            workbook.Save("MarkerForegroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


