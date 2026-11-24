---
title: "Cells.GetMaxGroupedColumnOutlineLevel"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Methode. Gibt die maximal gruppierte Spalten-Gliederungsebene (nullbasiert) zurück"
type: docs
url: /de/net/aspose.cells/cells/getmaxgroupedcolumnoutlinelevel/
---
## Cells.GetMaxGroupedColumnOutlineLevel method

Gibt die maximale gruppierte Spalten‑Gliederungsebene (nullbasiert) zurück.

```csharp
public int GetMaxGroupedColumnOutlineLevel()
```

### Rückgabewert

Die maximale gruppierte Spalten-Gliederungsebene (nullbasiert)

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsMethodGetMaxGroupedColumnOutlineLevelDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Gruppiere einige Spalten, um Gliederungsebenen zu demonstrieren
            cells.GroupColumns(0, 2, false);
            cells.GroupColumns(3, 5, false);
            
            // Erhalte die maximale gruppierte Spalten-Gliederungsebene
            int maxOutlineLevel = cells.GetMaxGroupedColumnOutlineLevel();
            
            Console.WriteLine("Maximum grouped column outline level: " + maxOutlineLevel);
            
            // Zeige die Gliederungsebene für jede Spalte an
            for (int col = 0; col < 6; col++)
            {
                int outlineLevel = cells.GetGroupedColumnOutlineLevel(col);
                Console.WriteLine($"Column {col} outline level: {outlineLevel}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("GroupedColumnsOutlineLevel.xlsx");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


