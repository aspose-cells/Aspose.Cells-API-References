---
title: "Cells.MaxColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells property. Maximaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden, schließt die Spalte nicht ein, für die der Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde."
type: docs
url: /de/net/aspose.cells/cells/maxcolumn/
---
## Cells.MaxColumn property

Maximaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte, für die ein Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde, nicht ein).

```csharp
public int MaxColumn { get; }
```

### Hinweise

Gibt -1 zurück, wenn keine Zelle instanziiert wurde.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMaxColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Einige Daten zu den Zellen hinzufügen
            worksheet.Cells["A1"].PutValue("Column A");
            worksheet.Cells["B1"].PutValue("Column B");
            worksheet.Cells["C1"].PutValue("Column C");
            
            // Ermitteln Sie den maximalen Spaltenindex mit Daten
            int maxColumn = worksheet.Cells.MaxColumn;
            Console.WriteLine("Max column with data: " + maxColumn);

            // Fügen Sie Daten zur nächsten Spalte nach der Max-Spalte hinzu
            worksheet.Cells[0, maxColumn + 1].PutValue("Next Column");

            // Überprüfen Sie die neue Max-Spalte
            Console.WriteLine("New max column: " + worksheet.Cells.MaxColumn);

            // Erstellen Sie ein weiteres Arbeitsblatt, um das Kopieren zu demonstrieren
            Worksheet destSheet = workbook.Worksheets.Add("Destination");

            // Kopieren Sie alle Spalten von der Quelle zum Ziel
            destSheet.Cells.CopyColumns(worksheet.Cells, 0, 0, worksheet.Cells.MaxColumn + 1);

            Console.WriteLine("Columns copied successfully");
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


