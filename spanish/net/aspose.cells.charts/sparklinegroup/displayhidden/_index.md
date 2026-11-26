---
title: "SparklineGroup.DisplayHidden"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad SparklineGroup. Indica si se deben mostrar datos en filas y columnas ocultas"
type: docs
url: /es/net/aspose.cells.charts/sparklinegroup/displayhidden/
---
## SparklineGroup.DisplayHidden property

Indica si se deben mostrar datos en filas y columnas ocultas.

```csharp
public bool DisplayHidden { get; set; }
```

### Ejemplos

```csharp
using System;
using System.Drawing;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklineGroupPropertyDisplayHiddenDemo
    {
        public static void Run()
        {
            // Crear un nuevo libro de trabajo
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo
            sheet.Cells["A1"].PutValue(5);
            sheet.Cells["B1"].PutValue(2);
            sheet.Cells["C1"].PutValue(1);
            sheet.Cells["D1"].PutValue(3);

            // Definir la ubicación del sparkline
            CellArea ca = new CellArea
            {
                StartColumn = 4,
                EndColumn = 4,
                StartRow = 0,
                EndRow = 0
            };

            // Agregar grupo de sparkline
            int idx = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[idx];

            // Agregar sparkline al grupo
            group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);

            // Configurar la apariencia del sparkline
            CellsColor seriesColor = workbook.CreateCellsColor();
            seriesColor.Color = Color.Blue;
            group.SeriesColor = seriesColor;

            // Demostrar la propiedad DisplayHidden
            group.DisplayHidden = true; // Show sparklines for hidden data

            // Guarda el libro de trabajo
            workbook.Save("SparklineDisplayHiddenDemo.xlsx");
        }
    }
}
```

### Ver también

* class [SparklineGroup](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


