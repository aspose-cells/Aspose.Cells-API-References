---
title: "ErrorBar.ShowMarkerTTop"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ErrorBar. Indica si se formatean las barras de error con un Ttop"
type: docs
url: /es/net/aspose.cells.charts/errorbar/showmarkerttop/
---
## ErrorBar.ShowMarkerTTop property

Indica si se formatean las barras de error con una T en la parte superior.

```csharp
public bool ShowMarkerTTop { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;
using Aspose.Cells.Drawing;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyShowMarkerTTopDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Agregar datos de ejemplo
            cells["A1"].PutValue(10);
            cells["A2"].PutValue(20);
            cells["A3"].PutValue(30);
            cells["B1"].PutValue(2);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(1);

            // Crear un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Establecer datos del gráfico
            chart.NSeries.Add("A1:A3", true);
            chart.NSeries.CategoryData = "B1:B3";

            // Configurar barras de error para la primera serie
            Series series = chart.NSeries[0];
            series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
            series.YErrorBar.Type = ErrorBarType.Percent;
            series.YErrorBar.Amount = 10;
            
            // Demostrar la propiedad ShowMarkerTTop
            series.YErrorBar.ShowMarkerTTop = true;
            series.YErrorBar.Color = System.Drawing.Color.Red;
            series.YErrorBar.Style = LineType.DashDot;

            // Guarda el libro de trabajo
            workbook.Save("ErrorBarShowMarkerTTopDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


