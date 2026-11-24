---
title: "Klasse HorizontalPageBreak"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.HorizontalPageBreak Klasse. Kapselt das Objekt, das einen horizontalen Seitenumbruch darstellt"
type: docs
url: /de/net/aspose.cells/horizontalpagebreak/
---
## HorizontalPageBreak class

Kapselt das Objekt, das einen horizontalen Seitenumbruch darstellt.

```csharp
public class HorizontalPageBreak
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [EndColumn](../../aspose.cells/horizontalpagebreak/endcolumn/) { get; } | Gibt den Endspaltenindex dieses horizontalen Seitenumbruchs zurück. |
| [Row](../../aspose.cells/horizontalpagebreak/row/) { get; } | Gibt den nullbasierten Zeilenindex zurück. |
| [StartColumn](../../aspose.cells/horizontalpagebreak/startcolumn/) { get; } | Gibt den Startspaltenindex dieses horizontalen Seitenumbruchs zurück. |

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class HorizontalPageBreakDemo
    {
        public static void HorizontalPageBreakExample()
        {
            // Instanziieren eines Workbook-Objekts
            Workbook workbook = new Workbook();
            
            // Abrufen der Referenz des neu hinzugefügten Arbeitsblatts durch Übergabe seines Blattindexes
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie einen Seitenumbruch bei Zelle Y30 hinzu
            int index = worksheet.HorizontalPageBreaks.Add("Y30");
            
            // Holen Sie den neu hinzugefügten horizontalen Seitenumbruch
            HorizontalPageBreak hPageBreak = worksheet.HorizontalPageBreaks[index];
            
            // Zeigen Sie die Eigenschaften des horizontalen Seitenumbruchs an
            Console.WriteLine("Horizontal Page Break Details:");
            Console.WriteLine($"Row: {hPageBreak.Row}");
            Console.WriteLine($"Start Column: {hPageBreak.StartColumn}");
            Console.WriteLine($"End Column: {hPageBreak.EndColumn}");
            
            // Speichere die Arbeitsmappe
            workbook.Save("HorizontalPageBreakExample.xlsx");
            workbook.Save("HorizontalPageBreakExample.pdf");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


