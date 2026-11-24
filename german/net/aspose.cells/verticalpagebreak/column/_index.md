---
title: "VerticalPageBreak.Column"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VerticalPageBreak-Eigenschaft. Gibt den Spaltenindex des vertikalen Seitenumbruchs zurück"
type: docs
url: /de/net/aspose.cells/verticalpagebreak/column/
---
## VerticalPageBreak.Column property

Liefert den Spaltenindex des vertikalen Seitenumbruchs.

```csharp
public int Column { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Vertikale Seitenumbrüche bei den Spalten 4 und 8 hinzufügen
            worksheet.VerticalPageBreaks.Add(4);
            worksheet.VerticalPageBreaks.Add(8);

            // Rufen Sie die Sammlung der vertikalen Seitenumbrüche ab
            VerticalPageBreakCollection vpagebreaks = worksheet.VerticalPageBreaks;

            // Informationen zu jedem vertikalen Seitenumbruch anzeigen
            Console.WriteLine("Vertical Page Breaks Count: " + vpagebreaks.Count);
            
            foreach (VerticalPageBreak vpagebreak in vpagebreaks)
            {
                Console.WriteLine("\nPage Break at Column: " + vpagebreak.Column);
                Console.WriteLine("Start Row: " + vpagebreak.StartRow);
                Console.WriteLine("End Row: " + vpagebreak.EndRow);
            }

            // Speichere die Arbeitsmappe
            workbook.Save("VerticalPageBreakDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


