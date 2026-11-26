---
title: "ErrorBar.PlusValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ErrorBar. Representa la cantidad de error positiva cuando el tipo de barra de error es Personalizado"
type: docs
url: /es/net/aspose.cells.charts/errorbar/plusvalue/
---
## ErrorBar.PlusValue property

Representa la cantidad de error positivo cuando el tipo de barra de error es Personalizado.

```csharp
public string PlusValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyPlusValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Series 1");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(30);
            worksheet.Cells["B4"].PutValue(40);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Establecer rango de datos del gráfico
            chart.NSeries.Add("B2:B4", true);

            // Configurar barras de error
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";  // Using PlusValue property
            errorBar.MinusValue = "=A3";

            // Guarda el libro de trabajo
            workbook.Save("ErrorBarPlusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


