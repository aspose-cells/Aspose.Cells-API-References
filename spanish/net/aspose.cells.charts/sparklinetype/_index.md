---
title: "Enumeración SparklineType"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Aspose.Cells.Charts.SparklineType enum. Representa los tipos de sparkline."
type: docs
url: /es/net/aspose.cells.charts/sparklinetype/
---
## SparklineType enumeration

Representa los tipos de sparkline.

```csharp
public enum SparklineType
```

### Valores

| Nombre | Valor | Descripción |
| --- | --- | --- |
| Line | `0` | Sparkline de línea. |
| Column | `1` | Sparkline de columna. |
| Stacked | `2` | Representa una sparkline de Ganancia/Pérdida. |
| WinLoss | `2` | Representa una sparkline de Ganancia/Pérdida. |

### Ejemplos

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Charts;
    using System;
    using System.Drawing;

    public class SparklineTypeDemo
    {
        public static void SparklineTypeExample()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Agregar algunos datos a la hoja de cálculo
            worksheet.Cells["A1"].PutValue(5);
            worksheet.Cells["B1"].PutValue(2);
            worksheet.Cells["C1"].PutValue(1);
            worksheet.Cells["D1"].PutValue(3);

            // Define el CellArea para el sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Añade un grupo de sparkline a la hoja de cálculo
            int idx = worksheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = worksheet.SparklineGroups[idx];

            // Añade sparklines al grupo
            group.Sparklines.Add(worksheet.Name + "!A1:D1", 0, 4);

            // Personaliza el grupo de sparkline
            CellsColor clr = workbook.CreateCellsColor();
            clr.Color = Color.Orange;
            group.SeriesColor = clr;

            // Establece que los puntos altos se coloreen de verde y los puntos bajos de rojo
            group.ShowHighPoint = true;
            group.ShowLowPoint = true;
            group.HighPointColor.Color = Color.Green;
            group.LowPointColor.Color = Color.Red;

            // Establece el grosor de la línea
            group.LineWeight = 1.0;

            // Guarda el libro de trabajo
            workbook.Save("SparklineTypeExample.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Ver también

* namespace [Aspose.Cells.Charts](../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../)


