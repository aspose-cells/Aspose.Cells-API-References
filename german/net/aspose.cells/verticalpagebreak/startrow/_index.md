---
title: "VerticalPageBreak.StartRow"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "VerticalPageBreak-Eigenschaft. Gibt den Startzeilenindex des vertikalen Seitenumbruchs zurück"
type: docs
url: /de/net/aspose.cells/verticalpagebreak/startrow/
---
## VerticalPageBreak.StartRow property

Liefert den Startzeilenindex des vertikalen Seitenumbruchs.

```csharp
public int StartRow { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class VerticalPageBreakPropertyStartRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge vertikale Seitenumbrüche mit der gewünschten Startzeile (2) initial hinzu
            worksheet.VerticalPageBreaks.Add(2, 0, 10);
            VerticalPageBreak vPageBreak = worksheet.VerticalPageBreaks[0];

            // Zeige die StartRow-Eigenschaft an
            Console.WriteLine("Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Da StartRow schreibgeschützt ist, müssen wir es entfernen und erneut hinzufügen, um es zu ändern
            worksheet.VerticalPageBreaks.RemoveAt(0);
            worksheet.VerticalPageBreaks.Add(5, 0, 10);
            vPageBreak = worksheet.VerticalPageBreaks[0];
            Console.WriteLine("Modified Vertical Page Break Start Row: " + vPageBreak.StartRow);

            // Speichere die Arbeitsmappe
            workbook.Save("VerticalPageBreakExample.xlsx");
        }
    }
}
```

### Siehe auch

* class [VerticalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


