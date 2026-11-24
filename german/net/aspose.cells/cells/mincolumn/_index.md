---
title: "Cells.MinColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Cells property. Minimaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden, schließt die Spalte nicht ein, für die der Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde."
type: docs
url: /de/net/aspose.cells/cells/mincolumn/
---
## Cells.MinColumn property

Minimaler Spaltenindex jener Zellen, die in der Sammlung instanziiert wurden (schließt die Spalte, für die ein Stil für die gesamte Spalte definiert ist, aber in der keine Zelle instanziiert wurde, nicht ein).

```csharp
public int MinColumn { get; }
```

### Hinweise

Diese Eigenschaft muss dynamisch Zellen und Zeilen iterieren und prüfen, daher ist sie zeitaufwendig und sollte nicht wiederholt aufgerufen werden, etwa indem sie direkt als Bedingung in einer Schleife verwendet wird.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsPropertyMinColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Auf die Cells-Sammlung zugreifen
            Cells cells = worksheet.Cells;
            
            // Füllen Sie einige Daten in den Spalten 2, 3 und 4 (B, C, D) ein
            cells["B1"].PutValue("Data in Column B");
            cells["C1"].PutValue("Data in Column C");
            cells["D1"].PutValue("Data in Column D");
            
            // Ermitteln Sie den minimalen Spaltenindex, der Daten enthält
            int minColumn = cells.MinColumn;
            
            // Ermitteln Sie den maximalen Spaltenindex, der Daten enthält
            int maxColumn = cells.MaxColumn;
            
            Console.WriteLine("Minimum column with data: " + minColumn); // Should output 1 (column B)
            Console.WriteLine("Maximum column with data: " + maxColumn); // Should output 3 (column D)
            
            // Spalte B leeren, um die Änderung von MinColumn zu demonstrieren
            cells.DeleteColumn(1);
            
            Console.WriteLine("\nAfter deleting column B:");
            Console.WriteLine("New minimum column with data: " + cells.MinColumn); // Should now output 2 (column C)
            Console.WriteLine("Maximum column with data: " + cells.MaxColumn); // Should still output 3 (column D)
        }
    }
}
```

### Siehe auch

* class [Cells](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


