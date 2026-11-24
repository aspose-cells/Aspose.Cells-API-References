---
title: "DeleteBlankOptions.EndIndex"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "DeleteBlankOptions-Eigenschaft. Gibt den End‑Zeilen‑/Spaltenindex des zu prüfenden und zu löschenden Bereichs an. Der Standardwert ist 1, und 1 bedeutet den maximalen Bereich aller Objekte/Zellen/Zeichnungen ... die überprüft werden müssen"
type: docs
url: /de/net/aspose.cells/deleteblankoptions/endindex/
---
## DeleteBlankOptions.EndIndex property

Gibt den End‑Zeilen‑/Spalten‑Index (einschließlich) des zu prüfenden Bereichs zum Löschen leerer Zeilen/Spalten an. Standardwert ist -1, wobei -1 den maximalen Bereich aller zu prüfenden Objekte (Zellen, Zeichnungen, …) bedeutet.

```csharp
public int EndIndex { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DeleteBlankOptionsPropertyEndIndexDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Cells cells = wb.Worksheets[0].Cells;

            // Füllen Sie einige Zellen mit Werten
            cells[0, 2].PutValue(2);
            cells[0, 5].PutValue(5);
            cells[0, 9].PutValue(9);

            // Erstellen Sie DeleteBlankOptions mit einem bestimmten Bereich
            DeleteBlankOptions dbo = new DeleteBlankOptions();
            dbo.StartIndex = 4;
            dbo.EndIndex = 7;

            // Löschen Sie leere Spalten im angegebenen Bereich
            cells.DeleteBlankColumns(dbo);

            // Geben Sie Ergebnisse aus, um die Wirkung von EndIndex zu demonstrieren
            Console.WriteLine("Value at C1: " + cells[0, 2].IntValue);
            Console.WriteLine("Value at F1 (originally G1): " + cells[0, 4].IntValue);
            Console.WriteLine("Value at G1 (originally K1): " + cells[0, 6].IntValue);
        }
    }
}
```

### Siehe auch

* class [DeleteBlankOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


