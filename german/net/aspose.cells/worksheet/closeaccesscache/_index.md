---
title: "Worksheet.CloseAccessCache"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Schließt die Sitzung, die Caches verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen"
type: docs
url: /de/net/aspose.cells/worksheet/closeaccesscache/
---
## Worksheet.CloseAccessCache method

Schließt die Sitzung, die Caches verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen.

```csharp
public void CloseAccessCache(AccessCacheOptions opts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | AccessCacheOptions | Optionen für den Datenzugriff |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            Cells cells = sheet.Cells;
            
            // Zellen mit Beispieldaten füllen
            for (int i = 0; i < 1000; i++)
            {
                cells[i, 0].PutValue(i % 10);
            }

            // Bedingte Formatierung hinzufügen
            FormatConditionCollection fcs = sheet.ConditionalFormattings[sheet.ConditionalFormattings.Add()];
            fcs.AddArea(CellArea.CreateCellArea(0, 0, 999, 0));
            fcs.AddCondition(FormatConditionType.ColorScale);

            // Zugriffscache für bedingte Formatierung aktivieren
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Operationen mit zwischengespeichertem Zugriff ausführen
            Random random = new Random();
            for (int i = 0; i < 100; i++)
            {
                int r = random.Next(0, 1000);
                var style = cells[r, 0].GetDisplayStyle();
                Console.WriteLine($"Cell ({r},0) style: {style.ForegroundArgbColor:X}");
            }

            // Den Zugriffscache schließen
            sheet.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);
        }
    }
}
```

### Siehe auch

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


