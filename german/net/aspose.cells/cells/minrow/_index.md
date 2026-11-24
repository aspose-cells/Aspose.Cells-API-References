---
title: "Cells.MinRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells-Eigenschaft. Minimaler Zeilenindex einer Zelle, die Daten oder Stil enthält"
type: docs
url: /de/net/aspose.cells/cells/minrow/
---
## Cells.MinRow property

Minimaler Zeilenindex der Zelle, die Daten oder einen Stil enthält.

```csharp
public int MinRow { get; }
```

### Hinweise

Diese Eigenschaft muss dynamisch Zellen und Zeilen iterieren und prüfen, daher ist sie zeitaufwendig und sollte nicht wiederholt aufgerufen werden, etwa indem sie direkt als Bedingung in einer Schleife verwendet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Einige Daten hinzufügen, um MinRow zu demonstrieren
            cells["A1"].PutValue("Data in first row");
            cells["B5"].PutValue("Data in fifth row");

            // MinRow-Informationen anzeigen
            Console.WriteLine("Minimum used row: " + cells.MinRow);
            Console.WriteLine("Maximum used row: " + cells.MaxRow);

            // Inhalte ab MinRow löschen
            cells.ClearContents(cells.MinRow, cells.MinColumn, cells.MaxRow, cells.MaxColumn);

            // Löschen überprüfen, indem geprüft wird, ob Zellen leer sind
            Console.WriteLine("A1 after clearing: " + (cells["A1"].Value == null ? "Empty" : "Not empty"));
            Console.WriteLine("B5 after clearing: " + (cells["B5"].Value == null ? "Empty" : "Not empty"));
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


