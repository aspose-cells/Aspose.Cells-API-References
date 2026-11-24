---
title: "Klasse Top10Filter"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Aspose.Cells.Top10Filter Klasse. Stellt die obersten N Prozent oder die Anzahl der zu filternden Elemente dar"
type: docs
url: /de/net/aspose.cells/top10filter/
---
## Top10Filter class

Stellt das oberste N (Prozent oder Anzahl der Elemente) zum Filtern dar.

```csharp
public class Top10Filter
```

## Eigenschaften

| Name | Beschreibung |
| --- | --- |
| [Criteria](../../aspose.cells/top10filter/criteria/) { get; set; } | (**Veraltet.**) Der tatsächliche Zellenwert im Bereich, der für den Vergleich dieses Filters verwendet wird. Dies ist der Cache-Wert während des Aktualisierungsvorgangs. |
| [IsPercent](../../aspose.cells/top10filter/ispercent/) { get; set; } | Gibt an, ob nach Prozentwert der Spalte gefiltert werden soll oder nicht |
| [IsTop](../../aspose.cells/top10filter/istop/) { get; set; } | Gibt an, ob nach oberster Reihenfolge gefiltert werden soll oder nicht |
| [Items](../../aspose.cells/top10filter/items/) { get; set; } | Liest und setzt den oberen oder unteren Wert, der als Filterkriterium verwendet wird. |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassTop10FilterDemo
    {
        public static void Run()
        {
            // Erstellen Sie eine Arbeitsmappe mit Beispieldaten
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Fügen Sie Beispieldaten hinzu
            worksheet.Cells["B6"].PutValue("Value");
            for (int i = 7; i <= 16; i++)
            {
                worksheet.Cells["B" + i].PutValue(20 - i);
                worksheet.Cells["C" + i].PutValue("Item " + (i-6));
            }
            
            // Wenden Sie Auto-Filter und Top‑10‑Filter an
            worksheet.AutoFilter.Range = "B6:C16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5); // Filter top 5 values in column B
            
            // Rufen Sie den Top10Filter ab und überprüfen Sie dessen Eigenschaften
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent);
            Console.WriteLine("Items: " + filter.Items);
            
            // Aktualisieren Sie den Filter und prüfen Sie versteckte Zeilen
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
            
            // Speichere die Arbeitsmappe
            workbook.Save("Top10FilterDemo.xlsx");
        }
    }
}
```

### Siehe auch

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


