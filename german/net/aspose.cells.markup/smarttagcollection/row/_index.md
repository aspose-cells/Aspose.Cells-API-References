---
title: "SmartTagCollection.Row"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "SmartTagCollection-Eigenschaft. Gibt die Zeile der Zellen‑SmartTags zurück"
type: docs
url: /de/net/aspose.cells.markup/smarttagcollection/row/
---
## SmartTagCollection.Row property

Ruft die Zeile der Zellen‑SmartTags ab.

```csharp
public int Row { get; }
```

### Beispiele

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagCollectionPropertyRowDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Füge einen SmartTag zur Zelle A1 (Zeile 0, Spalte 0) hinzu
            worksheet.Cells["A1"].PutValue("Sample with SmartTag");
            int index = worksheet.SmartTagSetting.Add("A1");
            
            // Rufe die SmartTagCollection für die Zelle A1 ab
            SmartTagCollection smartTags = worksheet.SmartTagSetting[index];

            // Zeige die Zeile der Zelle an, die diese SmartTags enthält
            Console.WriteLine("SmartTags are located at row: " + smartTags.Row);

            // Hinweis: Die Row‑Eigenschaft ist schreibgeschützt, daher können wir sie nicht setzen
            // smartTags.Row = 5; // Dies würde einen Kompilierungsfehler verursachen

            // Füge einen weiteren SmartTag zur Zelle B3 (Zeile 2, Spalte 1) hinzu, um eine andere Zeile zu demonstrieren
            worksheet.Cells["B3"].PutValue("Another SmartTag");
            int index2 = worksheet.SmartTagSetting.Add("B3");
            SmartTagCollection smartTags2 = worksheet.SmartTagSetting[index2];
            Console.WriteLine("Second SmartTags are located at row: " + smartTags2.Row);

            // Speichere die Arbeitsmappe
            workbook.Save("SmartTagRowDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [SmartTagCollection](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


