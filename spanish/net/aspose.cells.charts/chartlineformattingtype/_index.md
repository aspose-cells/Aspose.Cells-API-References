---
title: "Enum ChartLineFormattingType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.ChartLineFormattingType enum. Representa el tipo de formato de línea del gráfico"
type: docs
url: /es/net/aspose.cells.charts/chartlineformattingtype/
---
## ChartLineFormattingType enumeration

Representa el tipo de formato de línea de la línea del gráfico.

```csharp
public enum ChartLineFormattingType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Automatic | `0` | Representa el tipo de formato automático. |
| Solid | `1` | Representa el tipo de formato sólido. |
| None | `2` | Representa el tipo de formato ninguno. |
| Gradient | `3` | Gradiente |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class ChartLineFormattingTypeDemo
    {
        public static void ChartLineFormattingTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de muestra a las celdas
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            
            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Line, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];
            
            // Agregar series al gráfico
            chart.NSeries.Add("A1:B3", true);
            
            // Establecer los datos de la categoría
            chart.NSeries.CategoryData = "A1:A3";
            
            // Establecer diferentes tipos de formato de línea para la serie
            chart.NSeries[0].SeriesLines.FormattingType = ChartLineFormattingType.Solid;
            chart.NSeries[0].SeriesLines.Color = Color.Red;
            
            // Agregar otra serie con formato diferente
            chart.NSeries.Add("B1:B3", true);
            chart.NSeries[1].SeriesLines.FormattingType = ChartLineFormattingType.Gradient;
            chart.NSeries[1].SeriesLines.Color = Color.Blue;
            
            // Guarda el libro de trabajo
            workbook.Save("ChartLineFormattingTypeExample.xlsx");
            workbook.Save("ChartLineFormattingTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


