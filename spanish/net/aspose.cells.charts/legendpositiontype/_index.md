---
title: "Enum LegendPositionType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.LegendPositionType enum. Enumera los tipos de posición de la leyenda"
type: docs
url: /es/net/aspose.cells.charts/legendpositiontype/
---
## LegendPositionType enumeration

Enumera los tipos de posición de la leyenda.

```csharp
public enum LegendPositionType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Bottom | `0` | Muestra la leyenda en la parte inferior del área de trazado del gráfico. |
| Corner | `1` | Muestra la leyenda en la esquina del área de trazado del gráfico. |
| Left | `4` | Muestra la leyenda a la izquierda del área de trazado del gráfico. |
| NotDocked | `7` | Indica que la leyenda no está acoplada. |
| Right | `3` | Muestra la leyenda a la derecha del área de trazado del gráfico. |
| Top | `2` | Muestra la leyenda en la parte superior del área de trazado del gráfico. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;

    public class LegendPositionTypeDemo
    {
        public static void LegendPositionTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la hoja de cálculo
            Cells cells = sheet.Cells;
            cells[0, 1].PutValue("Income");
            cells[1, 0].PutValue("Company A");
            cells[2, 0].PutValue("Company B");
            cells[3, 0].PutValue("Company C");
            cells[1, 1].PutValue(10000);
            cells[2, 1].PutValue(20000);
            cells[3, 1].PutValue(30000);

            // Agregar un gráfico de columnas a la hoja de cálculo
            int chartIndex = sheet.Charts.Add(ChartType.Column, 9, 9, 21, 15);
            Chart chart = sheet.Charts[chartIndex];
            chart.SetChartDataRange("A1:B4", true);

            // Accede a la leyenda del gráfico
            Legend legend = chart.Legend;

            // Establecer la posición de la leyenda a la izquierda del gráfico
            legend.Position = LegendPositionType.Left;

            // Establecer propiedades adicionales para la leyenda
            legend.Y = 1500;
            legend.Width = 50;
            legend.Height = 50;

            // Guarda el libro de trabajo
            workbook.Save("LegendPositionTypeExample.xlsx");
            workbook.Save("LegendPositionTypeExample.pdf");
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


