---
title: "Enum ErrorBarDisplayType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Enum Aspose.Cells.Charts.ErrorBarDisplayType. Representa el tipo de visualización de la barra de error"
type: docs
url: /es/net/aspose.cells.charts/errorbardisplaytype/
---
## ErrorBarDisplayType enumeration

Representa el tipo de visualización de la barra de error.

```csharp
public enum ErrorBarDisplayType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Both | `0` | Ambos |
| Minus | `1` | Menos |
| None | `2` | Ninguno |
| Plus | `3` | Más |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarDisplayTypeDemo
    {
        public static void ErrorBarDisplayTypeExample()
        {
            // Crear un nuevo libro de trabajo y acceder a la primera hoja de cálculo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(2);
            worksheet.Cells["A2"].PutValue(5);
            worksheet.Cells["A3"].PutValue(3);
            worksheet.Cells["A4"].PutValue(6);
            worksheet.Cells["B1"].PutValue(4);
            worksheet.Cells["B2"].PutValue(3);
            worksheet.Cells["B3"].PutValue(6);
            worksheet.Cells["B4"].PutValue(7);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Agregar un gráfico de columnas a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = worksheet.Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Configurar barras de error para cada serie en el gráfico
            foreach (Series series in chart.NSeries)
            {
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Guarda el libro de trabajo
            workbook.Save("ErrorBarDisplayTypeExample.xlsx");
            workbook.Save("ErrorBarDisplayTypeExample.pdf");
            return;
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


