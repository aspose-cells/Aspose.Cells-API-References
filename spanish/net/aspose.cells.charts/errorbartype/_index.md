---
title: "Enum ErrorBarType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.ErrorBarType enum. Representa el tipo de cantidad de barra de error"
type: docs
url: /es/net/aspose.cells.charts/errorbartype/
---
## ErrorBarType enumeration

Representa el tipo de cantidad de la barra de error.

```csharp
public enum ErrorBarType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Custom | `0` | Tipo de valor InnerCustom. |
| FixedValue | `1` | Tipo de valor fijo. |
| Percent | `2` | Tipo de porcentaje |
| StDev | `3` | Tipo de desviación estándar. |
| StError | `4` | Tipo de error estándar. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class ErrorBarTypeDemo
    {
        public static void ErrorBarTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Agregar algunos datos de ejemplo
            cells["A1"].PutValue(2);
            cells["A2"].PutValue(5);
            cells["A3"].PutValue(3);
            cells["A4"].PutValue(6);
            cells["B1"].PutValue(4);
            cells["B2"].PutValue(3);
            cells["B3"].PutValue(6);
            cells["B4"].PutValue(7);

            cells["C1"].PutValue("Q1");
            cells["C2"].PutValue("Q2");
            cells["C3"].PutValue("Y1");
            cells["C4"].PutValue("Y2");

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = workbook.Worksheets[0].Charts.Add(ChartType.Column, 11, 0, 27, 10);
            Chart chart = workbook.Worksheets[0].Charts[chartIndex];
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Establecer propiedades de la barra de error para cada serie en el gráfico
            for (int i = 0; i < chart.NSeries.Count; i++)
            {
                Series series = chart.NSeries[i];
                series.YErrorBar.DisplayType = ErrorBarDisplayType.Minus;
                series.YErrorBar.Type = ErrorBarType.FixedValue;
                series.YErrorBar.Amount = 5;
            }

            // Guarda el libro de trabajo
            workbook.Save("ErrorBarTypeExample.xlsx");
            workbook.Save("ErrorBarTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


