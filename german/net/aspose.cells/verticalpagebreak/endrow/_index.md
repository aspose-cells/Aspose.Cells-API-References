---
title: "VerticalPageBreak.EndRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VerticalPageBreak-Eigenschaft. Gibt den Endzeilenindex des vertikalen Seitenumbruchs zurück"
type: docs
url: /de/net/aspose.cells/verticalpagebreak/endrow/
---
## VerticalPageBreak.EndRow property

Liefert den Endzeilenindex des vertikalen Seitenumbruchs.

```csharp
public int EndRow { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyEndRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greife auf das erste Arbeitsblatt zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Einen vertikalen Seitenumbruch hinzufügen, der die Zeilen 3 bis 8 in Spalte C (Index 2) umfasst
            worksheet.VerticalPageBreaks.Add("C3:C8");

            // Den ersten vertikalen Seitenumbruch abrufen
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];
            
            // Den Endzeilenwert des Seitenumbruchs anzeigen
            Console.WriteLine("Vertical Page Break End Row: " + vpb.EndRow);
            
            // Da EndRow schreibgeschützt ist, zeigen wir das Abrufen, aber nicht das Setzen.
            // Die folgende Zeile wird entfernt, da sie einen Kompilierungsfehler verursacht:
            // vpb.EndRow = 10;
            
            // Stattdessen fügen wir einen weiteren Seitenumbruch mit einer anderen Endzeile hinzu
            worksheet.VerticalPageBreaks.Add("C3:C10");
            VerticalPageBreak vpb2 = worksheet.VerticalPageBreaks[1];
            Console.WriteLine("Second Page Break End Row: " + vpb2.EndRow);
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


