---
title: "Cells.GetMaxGroupedRowOutlineLevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die maximal gruppierte Zeilen-Gliederungsebene nullbasiert zurück"
type: docs
url: /de/net/aspose.cells/cells/getmaxgroupedrowoutlinelevel/
---
## Cells.GetMaxGroupedRowOutlineLevel method

Gibt die maximale gruppierte Zeilen‑Gliederungsebene (nullbasiert) zurück.

```csharp
public int GetMaxGroupedRowOutlineLevel()
```

### Rückgabewert

Die maximale gruppierte Zeilen-Gliederungsebene (nullbasiert)

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedRowOutlineLevelDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Zeilen gruppieren, um Gliederungsebenen zu demonstrieren
            cells.GroupRows(0, 2, false);
            cells.GroupRows(4, 6, false);
            
            // Verschachtelte Gruppierung hinzufügen
            cells.GroupRows(4, 5, true);

            // Die maximale gruppierte Zeilen-Gliederungsebene abrufen
            int maxOutlineLevel = cells.GetMaxGroupedRowOutlineLevel();

            // Ergebnis anzeigen
            Console.WriteLine("Maximum grouped row outline level: " + maxOutlineLevel);

            // Gliederungsebene für jede Zeile anzeigen
            for (int row = 0; row <= 6; row++)
            {
                Console.WriteLine($"Row {row} outline level: {cells.GetGroupedRowOutlineLevel(row)}");
            }
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


