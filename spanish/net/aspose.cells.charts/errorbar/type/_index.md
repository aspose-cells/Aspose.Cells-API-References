---
title: "ErrorBar.Type"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ErrorBar. Representa el tipo de cantidad de la barra de error"
type: docs
url: /es/net/aspose.cells.charts/errorbar/type/
---
## ErrorBar.Type property

Representa el tipo de cantidad de la barra de error.

```csharp
public ErrorBarType Type { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyTypeDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook wb = new Workbook();
            Worksheet ws = wb.Worksheets[0];
            
            // Agregar datos de ejemplo
            ws.Cells["A1"].PutValue(5);
            ws.Cells["A2"].PutValue(3);
            
            // Crear un gráfico
            int chartIndex = ws.Charts.Add(ChartType.Line, 5, 0, 20, 10);
            Chart chart = ws.Charts[chartIndex];
            
            // Agregar datos de la serie
            chart.NSeries.Add("A3:A10", true);
            Series series = chart.NSeries[0];
            
            // Establecer tipo y valores personalizados de la barra de error
            series.YErrorBar.Type = ErrorBarType.Custom;
            series.YErrorBar.PlusValue = "=Sheet1!A1";
            series.YErrorBar.MinusValue = "=Sheet1!A2";
            
            // Guarda el libro de trabajo
            wb.Save("ErrorBarDemo.xlsx");
        }
    }
}
```

### Ver también

* enum [ErrorBarType](../../errorbartype/)
* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


