---
title: "Worksheet.GetSelectedAreas"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Ruft die ausgewählten Zellbereiche im Designer-Tabellenblatt ab"
type: docs
url: /de/net/aspose.cells/worksheet/getselectedareas/
---
## Worksheet.GetSelectedAreas method

Liest die ausgewählten Zellbereiche im Designer-Tabellenblatt.

```csharp
public Range[] GetSelectedAreas()
```

### Rückgabewert

Gibt alle ausgewählten Bereiche zurück.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodGetSelectedAreasDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Mehrere Bereiche auswählen
            worksheet.SelectRange(0, 0, 2, 2, false); // First range (A1:C3)
            worksheet.SelectRange(4, 4, 6, 6, false); // Second range (E5:G7)
            
            // Ausgewählte Bereiche abrufen
            Aspose.Cells.Range[] selectedAreas = worksheet.GetSelectedAreas();
            
            // Informationen zu ausgewählten Bereichen anzeigen
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            for (int i = 0; i < selectedAreas.Length; i++)
            {
                Console.WriteLine($"Area {i + 1}: {selectedAreas[i].Address}");
            }
            
            // Auswahlen löschen und einen einzelnen Bereich auswählen
            worksheet.SelectRange(1, 1, 3, 3, true); // New single selection (B2:D4)
            
            // Den einzelnen ausgewählten Bereich abrufen
            selectedAreas = worksheet.GetSelectedAreas();
            Console.WriteLine("\nAfter single selection:");
            Console.WriteLine("Number of selected areas: " + selectedAreas.Length);
            Console.WriteLine("Selected area: " + selectedAreas[0].Address);
        }
    }
}
```

### Siehe auch

* class [Range](../../range/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


