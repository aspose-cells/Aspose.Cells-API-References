---
title: "ErrorBar.DisplayType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ErrorBar. Representa el tipo de visualización de la barra de error"
type: docs
url: /es/net/aspose.cells.charts/errorbar/displaytype/
---
## ErrorBar.DisplayType property

Representa el tipo de visualización de la barra de error.

```csharp
public ErrorBarDisplayType DisplayType { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyDisplayTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("X");
            worksheet.Cells["A2"].PutValue(1);
            worksheet.Cells["A3"].PutValue(2);
            worksheet.Cells["A4"].PutValue(3);
            worksheet.Cells["B1"].PutValue("Y");
            worksheet.Cells["B2"].PutValue(10);
            worksheet.Cells["B3"].PutValue(20);
            worksheet.Cells["B4"].PutValue(30);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar serie
            chart.NSeries.Add("A2:A4", true);
            chart.NSeries.CategoryData = "B2:B4";

            // Establecer tipo de visualización de la barra de error
            chart.NSeries[0].YErrorBar.DisplayType = ErrorBarDisplayType.Plus;

            // Guarda el libro de trabajo
            workbook.Save("ErrorBarDisplayTypeDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* enum [ErrorBarDisplayType](../../errorbardisplaytype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


