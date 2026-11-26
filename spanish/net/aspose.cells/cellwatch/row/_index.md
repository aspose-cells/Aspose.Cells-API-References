---
title: "CellWatch.Row"
second_title: "Referencia de API de Aspose.Cells para .NET"
description: "Propiedad CellWatch. Obtiene y establece la fila de la celda"
type: docs
url: /es/net/aspose.cells/cellwatch/row/
---
## CellWatch.Row property

Obtiene y establece la fila de la celda.

```csharp
public int Row { get; set; }
```

### Ejemplos

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellWatchPropertyRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Agregar datos de ejemplo a la celda B2
            sheet.Cells["B2"].PutValue("Sample Data");

            // Agregar CellWatch para B2
            int watchIndex = sheet.CellWatches.Add("B2");
            CellWatch cellWatch = sheet.CellWatches[watchIndex];

            // Demostrar la propiedad Row
            Console.WriteLine($"Original Row: {cellWatch.Row}");
            cellWatch.Row = 1; // Set row to 1 (0-based) for B2
            Console.WriteLine($"Updated Row: {cellWatch.Row}");

            // Verifique la referencia de la celda
            Console.WriteLine($"Cell Reference: {sheet.Cells[cellWatch.Row, cellWatch.Column].Name}");

            workbook.Save("CellWatchRowDemo.xlsx");
        }
    }
}
```

### Ver también

* class [CellWatch](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


