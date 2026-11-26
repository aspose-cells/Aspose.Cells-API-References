---
title: "Sparkline.Column"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad Sparkline. Obtiene el índice de columna del sparkline"
type: docs
url: /es/net/aspose.cells.charts/sparkline/column/
---
## Sparkline.Column property

Obtiene el índice de columna del sparkline.

```csharp
public int Column { get; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Charts;

namespace AsposeCellsExamples
{
    public class SparklinePropertyColumnDemo
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
            CellArea ca = new CellArea();
            ca.StartRow = 0;
            ca.EndRow = 0;
            ca.StartColumn = 4;
            ca.EndColumn = 4;
            
            int groupIndex = sheet.SparklineGroups.Add(SparklineType.Line, "A1:D1", false, ca);
            SparklineGroup group = sheet.SparklineGroups[groupIndex];

            // Agregue sparkline en la columna 4 y demuestre la propiedad Column
            int sparklineIndex = group.Sparklines.Add("A1:D1", 0, 4);
            Sparkline sparkline = group.Sparklines[sparklineIndex];

            // Muestre la propiedad column (solo lectura)
            Console.WriteLine("Sparkline Column: " + sparkline.Column);

            // Para cambiar la posición de la columna, necesitamos eliminar y volver a agregar el sparkline
            group.Sparklines.RemoveAt(sparklineIndex);
            sparklineIndex = group.Sparklines.Add("A1:D1", 0, 5); // New column position
            sparkline = group.Sparklines[sparklineIndex];
            Console.WriteLine("New Sparkline Column: " + sparkline.Column);

            // Guardar el libro de trabajo
            workbook.Save("SparklineColumnDemo.xlsx");
        }
    }
}
```

### Ver también

* class [Sparkline](../)
* namespace [Aspose.Cells.Charts](../../../aspose.cells.charts/)
* assembly [Aspose.Cells](../../../)


