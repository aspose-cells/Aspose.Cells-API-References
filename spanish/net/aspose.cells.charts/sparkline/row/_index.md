---
title: "Sparkline.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Sparkline. Obtiene el índice de fila de la sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparkline/row/
---
## Sparkline.Row property

Obtiene el índice de fila del sparkline.

```csharp
public int Row { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyRowDemo
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

            // Crear grupo de sparkline
            CellArea ca = new CellArea
            {
                StartRow = 0,
                EndRow = 0,
                StartColumn = 4,
                EndColumn = 4
            };

            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, sheet.Name + "!A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Agregar sparkline en la fila 0, columna 4
            int sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Mostrar posición de fila (propiedad de solo lectura)
            Console.WriteLine("Sparkline row position: " + sparkline.Row);

            // Para cambiar la posición, necesitamos eliminar y recrear la sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add(sheet.Name + "!A1:D1", 2, 4); // New position at row 2
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New sparkline row position: " + sparkline.Row);

            // Guardar el libro de trabajo
            workbook.Save("SparklineRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


