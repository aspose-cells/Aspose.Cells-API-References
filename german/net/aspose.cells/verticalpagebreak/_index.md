---
title: "Klasse VerticalPageBreak"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.VerticalPageBreak‑Klasse. Kapselt das Objekt, das einen vertikalen Seitenumbruch darstellt"
type: docs
url: /de/net/aspose.cells/verticalpagebreak/
---
## VerticalPageBreak class

Kapselt das Objekt, das einen vertikalen Seitenumbruch darstellt.

```csharp
public class VerticalPageBreak
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Column](../../aspose.cells/verticalpagebreak/column/) { get; } | Liefert den Spaltenindex des vertikalen Seitenumbruchs. |
| [EndRow](../../aspose.cells/verticalpagebreak/endrow/) { get; } | Liefert den Endzeilenindex des vertikalen Seitenumbruchs. |
| [StartRow](../../aspose.cells/verticalpagebreak/startrow/) { get; } | Liefert den Startzeilenindex des vertikalen Seitenumbruchs. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class VerticalPageBreakDemo
    {
        public static void VerticalPageBreakExample()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Greifen Sie auf das erste Arbeitsblatt in der Arbeitsmappe zu
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Füge einen vertikalen Seitenumbruch in Spalte G (Index 6) hinzu
            worksheet.VerticalPageBreaks.Add("G5");

            // Speichere die Arbeitsmappe
            workbook.Save("VerticalPageBreakExample.xlsx");

            // Greife auf den hinzugefügten vertikalen Seitenumbruch zu
            VerticalPageBreak vpb = worksheet.VerticalPageBreaks[0];

            // Zeige die Eigenschaften des vertikalen Seitenumbruchs an
            Console.WriteLine("Start Row: " + vpb.StartRow);
            Console.WriteLine("End Row: " + vpb.EndRow);
            Console.WriteLine("Column: " + vpb.Column);
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


