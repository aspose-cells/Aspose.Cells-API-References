---
title: "ErrorBar.MinusValue"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad ErrorBar. Representa la cantidad de error negativa cuando el tipo de barra de error es Personalizado"
type: docs
url: /es/net/aspose.cells.charts/errorbar/minusvalue/
---
## ErrorBar.MinusValue property

Representa la cantidad de error negativo cuando el tipo de barra de error es Personalizado.

```csharp
public string MinusValue { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class ErrorBarPropertyMinusValueDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            worksheet.Cells["A1"].PutValue("Values");
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["A3"].PutValue(5);
            worksheet.Cells["B1"].PutValue("Data");
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["B3"].PutValue(15);

            // Añade un gráfico
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 20, 8);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar serie
            chart.NSeries.Add("B2:B3", true);

            // Configurar barras de error
            ErrorBar errorBar = chart.NSeries[0].YErrorBar;
            errorBar.DisplayType = ErrorBarDisplayType.Both;
            errorBar.Type = ErrorBarType.Custom;
            errorBar.PlusValue = "=A2";
            errorBar.MinusValue = "=A3";

            // Guarda el libro de trabajo
            workbook.Save("ErrorBarMinusValueDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* class [ErrorBar](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


