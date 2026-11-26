---
title: "Marker.BackgroundColorSetType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Marker. Obtiene o establece el tipo de conjunto de color de fondo del marcador"
type: docs
url: /es/net/aspose.cells.charts/marker/backgroundcolorsettype/
---
## Marker.BackgroundColorSetType property

Obtiene o establece el tipo de conjunto de color de fondo del marcador.

```csharp
public FormattingType BackgroundColorSetType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class MarkerPropertyBackgroundColorSetTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar serie
            int seriesIndex = chart.NSeries.Add("A1:B3", true);
            Series series = chart.NSeries[seriesIndex];

            // Configurar propiedades del marcador
            series.Marker.MarkerStyle = ChartMarkerType.Circle;
            series.Marker.BackgroundColorSetType = FormattingType.Automatic;
            series.Marker.BackgroundColor = System.Drawing.Color.Yellow;

            // Guarda el libro de trabajo
            workbook.Save("MarkerBackgroundColorSetTypeDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [FormattingType](../../formattingtype/)
* class [Marker](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


