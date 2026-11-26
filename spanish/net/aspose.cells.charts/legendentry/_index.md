---
title: "Clase LegendEntry"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.LegendEntry class. Representa una entrada de leyenda en la leyenda de un gráfico"
type: docs
url: /es/net/aspose.cells.charts/legendentry/
---
## LegendEntry class

Representa una entrada de leyenda en la leyenda del gráfico.

```csharp
public class LegendEntry
```

## Propiedades

| Nombre | Descripción |
| --- | --- |
| [AutoScaleFont](../../aspose.cells.charts/legendentry/autoscalefont/) { get; set; } | True si el texto en el objeto cambia el tamaño de fuente cuando cambia el tamaño del objeto. El valor predeterminado es True. |
| [Background](../../aspose.cells.charts/legendentry/background/) { get; set; } | (**Obsolete.**) Obtiene y establece el modo de visualización del fondo |
| [BackgroundMode](../../aspose.cells.charts/legendentry/backgroundmode/) { get; set; } | Obtiene y establece el modo de visualización del fondo |
| [Font](../../aspose.cells.charts/legendentry/font/) { get; } | Obtiene un objeto [`Font`](./font/) del objeto ChartFrame especificado. |
| [IsDeleted](../../aspose.cells.charts/legendentry/isdeleted/) { get; set; } | Obtiene y establece si la entrada de leyenda está eliminada. |
| [IsTextNoFill](../../aspose.cells.charts/legendentry/istextnofill/) { get; set; } | Obtiene o establece sin relleno el texto. |
| virtual [TextFont](../../aspose.cells.charts/legendentry/textfont/) { get; } | (**Obsolete.**) Obtiene un objeto [`Font`](./font/) del objeto LegendEntry especificado. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendEntryDemo
    {
        public static void LegendEntryExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            
            // Agregar una nueva hoja de cálculo al libro
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Agregar datos de ejemplo a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(50);
            worksheet.Cells["A2"].PutValue(100);
            worksheet.Cells["A3"].PutValue(150);
            worksheet.Cells["A4"].PutValue(200);
            worksheet.Cells["B1"].PutValue(60);
            worksheet.Cells["B2"].PutValue(32);
            worksheet.Cells["B3"].PutValue(50);
            worksheet.Cells["B4"].PutValue(40);
            worksheet.Cells["C1"].PutValue("Q1");
            worksheet.Cells["C2"].PutValue("Q2");
            worksheet.Cells["C3"].PutValue("Y1");
            worksheet.Cells["C4"].PutValue("Y2");

            // Agregar un gráfico a la hoja de cálculo
            int chartIndex = worksheet.Charts.Add(ChartType.Column, 5, 0, 15, 5);
            Chart chart = worksheet.Charts[chartIndex];

            // Agregar NSeries (fuente de datos del gráfico) al gráfico que abarca desde la celda "A1" hasta "B4"
            chart.NSeries.Add("A1:B4", true);
            chart.NSeries.CategoryData = "C1:C4";

            // Acceder a la entrada de leyenda de la primera serie
            LegendEntry legendEntry = chart.NSeries[0].LegendEntry;

            // Establecer propiedades de la entrada de leyenda
            legendEntry.IsDeleted = false;
            legendEntry.IsTextNoFill = false;
            legendEntry.AutoScaleFont = true;
            legendEntry.Background = BackgroundMode.Transparent;
            legendEntry.BackgroundMode = BackgroundMode.Opaque;

            // Acceder y modificar la fuente de la entrada de leyenda
            Font font = legendEntry.Font;
            font.Name = "Arial";
            font.Size = 12;
            font.IsBold = true;
            font.Color = System.Drawing.Color.Blue;

            // Guarda el libro de trabajo
            workbook.Save("LegendEntryExample.xlsx");
            workbook.Save("LegendEntryExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


