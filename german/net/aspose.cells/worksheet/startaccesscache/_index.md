---
title: "Worksheet.StartAccessCache"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Worksheet-Methode. Startet die Sitzung, die Caches verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen"
type: docs
url: /de/net/aspose.cells/worksheet/startaccesscache/
---
## Worksheet.StartAccessCache method

Startet die Sitzung, die Zwischenspeicher verwendet, um auf die Daten in diesem Arbeitsblatt zuzugreifen.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | AccessCacheOptions | Optionen für den Datenzugriff |

### Hinweise

Nach dem Abschluss des Datenzugriffs sollte [`CloseAccessCache`](../closeaccesscache/) mit denselben Optionen aufgerufen werden, um alle Caches zu leeren und den normalen Zugriffsmodus wiederherzustellen.

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Standardstil festlegen
            Style style = wb.DefaultStyle;
            style.Font.Size = 10;
            wb.DefaultStyle = style;

            // Bedingte Formatierung hinzufügen
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            FormatConditionCollection fcc = cfc[cfc.Add()];
            fcc.AddArea(CellArea.CreateCellArea(0, 0, 10, 10));
            fcc.AddCondition(FormatConditionType.DuplicateValues);
            FormatCondition fc = fcc[0];
            fc.Style.Font.Size = 16;

            // Einige Daten befüllen
            Cells cells = sheet.Cells;
            for (int i = 0; i < 10; i++)
            {
                cells[0, i].PutValue("A");
                cells[i, 0].PutValue(i);
            }

            // Zugriffscache starten für bessere Leistung
            sheet.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Stile überprüfen
            for (int i = 0; i < 10; i++)
            {
                Console.WriteLine($"Cell[0,{i}] Font Size: {cells[0, i].GetDisplayStyle().Font.Size}");
                Console.WriteLine($"Cell[{i},0] Font Size: {cells[i, 0].GetDisplayStyle().Font.Size}");
            }

            // Cache schließen, wenn fertig
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


