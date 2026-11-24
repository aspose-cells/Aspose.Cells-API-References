---
title: "Range.MoveTo"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Range-Methode. Verschiebt den aktuellen Bereich zum Zielbereich"
type: docs
url: /de/net/aspose.cells/range/moveto/
---
## Range.MoveTo method

Verschiebt den aktuellen Bereich zum Zielbereich.

```csharp
public void MoveTo(int destRow, int destColumn)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| destRow | Int32 | Die Startzeile des Zielbereichs. |
| destColumn | Int32 | Die Startspalte des Zielbereichs. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodMoveToWithInt32Int32Demo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Erstelle einen Beispielbereich (A1:B2)
            Aspose.Cells.Range originalRange = worksheet.Cells.CreateRange("A1", "B2");
            
            // Füge einige Daten in den Bereich zur Demonstration ein
            originalRange[0, 0].PutValue("A1");
            originalRange[0, 1].PutValue("B1");
            originalRange[1, 0].PutValue("A2");
            originalRange[1, 1].PutValue("B2");
            
            // Verschiebe den Bereich um 1 Zeile nach unten (zu A2:B3)
            originalRange.MoveTo(originalRange.FirstRow + 1, originalRange.FirstColumn);
            
            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


