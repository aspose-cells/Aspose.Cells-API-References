---
title: "HorizontalPageBreak.EndColumn"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "HorizontalPageBreak-Eigenschaft. Gibt den Endspaltenindex dieses horizontalen Seitenumbruchs zurück"
type: docs
url: /de/net/aspose.cells/horizontalpagebreak/endcolumn/
---
## HorizontalPageBreak.EndColumn property

Gibt den Endspaltenindex dieses horizontalen Seitenumbruchs zurück.

```csharp
public int EndColumn { get; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HorizontalPageBreakPropertyEndColumnDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen horizontalen Seitenumbruch in Zeile 5 hinzu, der sich von Spalte 2 bis 4 erstreckt
            int index = worksheet.HorizontalPageBreaks.Add(5, 2, 4);
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];

            // Zeige die EndColumn-Eigenschaft
            Console.WriteLine("Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);

            // Da EndColumn schreibgeschützt ist, müssen wir den Seitenumbruch entfernen und erneut hinzufügen, um ihn zu ändern
            worksheet.HorizontalPageBreaks.RemoveAt(index);
            index = worksheet.HorizontalPageBreaks.Add(5, 2, 6);
            hPageBreak = worksheet.HorizontalPageBreaks[index];
            Console.WriteLine("Modified Horizontal Page Break EndColumn: " + hPageBreak.EndColumn);
        }
    }
}
```

### Siehe auch

* class [HorizontalPageBreak](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


