---
title: "Top10Filter.IsTop"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Top10Filter‑Eigenschaft. Gibt an, ob nach oberster Reihenfolge gefiltert wird oder nicht"
type: docs
url: /de/net/aspose.cells/top10filter/istop/
---
## Top10Filter.IsTop property

Gibt an, ob nach oberster Reihenfolge gefiltert werden soll oder nicht

```csharp
public bool IsTop { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsTopDemo
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
            }

            // Top‑5‑Filter anwenden
            worksheet.AutoFilter.Range = "B6:B16";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Holen Sie den Filter und prüfen Sie die IsTop‑Eigenschaft
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop); // Should output "True"
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output "False"
            
            // Filter aktualisieren und versteckte Zeilen prüfen
            worksheet.AutoFilter.Refresh();
            for (int i = 6; i <= 16; i++)
            {
                Console.WriteLine($"Row {i} hidden: {worksheet.Cells.IsRowHidden(i)}");
            }
        }
    }
}
```

### Siehe auch

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


