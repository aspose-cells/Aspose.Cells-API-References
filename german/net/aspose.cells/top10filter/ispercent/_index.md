---
title: "Top10Filter.IsPercent"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Top10Filter-Eigenschaft. Gibt an, ob nach dem Prozentwert der Spalte gefiltert werden soll"
type: docs
url: /de/net/aspose.cells/top10filter/ispercent/
---
## Top10Filter.IsPercent property

Gibt an, ob nach Prozentwert der Spalte gefiltert werden soll oder nicht

```csharp
public bool IsPercent { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class Top10FilterPropertyIsPercentDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fügen Sie Beispieldaten hinzu
            for (int i = 0; i < 10; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].PutValue((i + 1) * (j + 1));
                }
            }

            // Top-10-Filter anwenden (nicht prozentual)
            worksheet.AutoFilter.Range = "A1:J10";
            worksheet.AutoFilter.FilterTop10(0, true, false, 5);
            
            // Den Filter abrufen und die IsPercent-Eigenschaft demonstrieren
            Top10Filter filter = worksheet.AutoFilter.FilterColumns[0].Filter as Top10Filter;
            Console.WriteLine("IsTop: " + filter.IsTop);
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output False

            // Top-10-Prozent-Filter anwenden
            worksheet.AutoFilter.FilterTop10(1, true, true, 20);
            filter = worksheet.AutoFilter.FilterColumns[1].Filter as Top10Filter;
            Console.WriteLine("IsPercent: " + filter.IsPercent); // Should output True
        }
    }
}
```

### Siehe auch

* class [Top10Filter](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


