---
title: "Cells.MinDataRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Minimaler Zeilenindex der Zelle, die Daten enthält"
type: docs
url: /de/net/aspose.cells/cells/mindatarow/
---
## Cells.MinDataRow property

Minimaler Zeilenindex der Zelle, die Daten enthält.

```csharp
public int MinDataRow { get; }
```

### Hinweise

Gibt -1 zurück, wenn keine Zelle Daten enthält. Diese Eigenschaft muss Zellen und Zeilen dynamisch durchlaufen und prüfen, daher ist sie zeitaufwendig und sollte nicht wiederholt aufgerufen werden, etwa indem sie direkt als Bedingung in einer Schleife verwendet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinDataRowDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Einige Daten befüllen
            sheet.Cells[0, 0].Value = "Header1";
            sheet.Cells[0, 1].Value = "Header2";
            sheet.Cells[1, 0].Value = "Data1";
            sheet.Cells[1, 1].Value = "Data2";
            sheet.Cells[2, 0].Value = "Data3";
            sheet.Cells[2, 1].Value = "Data4";

            // Demonstriere die Verwendung von MinDataRow
            Console.WriteLine("Minimum data row index: " + sheet.Cells.MinDataRow);
            Console.WriteLine("Maximum data row index: " + sheet.Cells.MaxDataRow);

            // Speichere die Arbeitsmappe
            workbook.Save("MinDataRowExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


