---
title: "Cells.IsDefaultRowHeightMatched"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Gibt an, dass Zeilenhöhe und Standard-Schriftgröße übereinstimmen"
type: docs
url: /de/net/aspose.cells/cells/isdefaultrowheightmatched/
---
## Cells.IsDefaultRowHeightMatched property

Gibt an, dass Zeilenhöhe und Standard‑Schriftgröße übereinstimmen.

```csharp
public bool IsDefaultRowHeightMatched { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyIsDefaultRowHeightMatchedDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;

            // Setze und demonstriere die IsDefaultRowHeightMatched-Eigenschaft
            cells.IsDefaultRowHeightMatched = true;
            Console.WriteLine("IsDefaultRowHeightMatched: " + cells.IsDefaultRowHeightMatched);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");

            // Laden Sie die gespeicherte Arbeitsmappe, um die Eigenschaft zu überprüfen
            Workbook loadedWorkbook = new Workbook("output.xlsx");
            Cells loadedCells = loadedWorkbook.Worksheets[0].Cells;
            Console.WriteLine("Loaded IsDefaultRowHeightMatched: " + loadedCells.IsDefaultRowHeightMatched);
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


