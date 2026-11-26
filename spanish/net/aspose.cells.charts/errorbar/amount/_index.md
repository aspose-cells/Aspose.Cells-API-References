---
title: "ErrorBar.Amount"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ErrorBar. Representa la cantidad de la barra de error"
type: docs
url: /es/net/aspose.cells.charts/errorbar/amount/
---
## ErrorBar.Amount property

Representa la cantidad de la barra de error.

```csharp
public double Amount { get; set; }
```

### Observaciones

La cantidad debe ser mayor o igual a cero.

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyAmountDemo
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
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 5, 15, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B3", true);

            // Configurar barras de error
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Both;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5; // Demonstrate Amount property
            }

            workbook.Save("ErrorBarAmountDemo.xlsx");
        }
    }
}
```

### Ver también

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


