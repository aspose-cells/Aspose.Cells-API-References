---
title: "Workbook.CloseAccessCache"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Schließt die Sitzung, die Caches zum Zugriff auf Daten verwendet"
type: docs
url: /de/net/aspose.cells/workbook/closeaccesscache/
---
## Workbook.CloseAccessCache method

Schließt die Sitzung, die Zwischenspeicher zum Datenzugriff verwendet.

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
    public class WorkbookMethodCloseAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Zugriff auf das erste Arbeitsblatt
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // Beispieldaten und bedingte Formatierung hinzufügen
            for (int i = 0; i < 10; i++)
            {
                cells[i, 0].PutValue(i % 2 == 0 ? "Data" : "Other");
            }

            // Bedingte Formatierung hinzufügen
            int ruleIdx = worksheet.ConditionalFormattings.Add();
            FormatConditionCollection fcc = worksheet.ConditionalFormattings[ruleIdx];
            fcc.AddCondition(FormatConditionType.CellValue, OperatorType.Equal, "Data", null);
            Style style = workbook.CreateStyle();
            style.Font.Size = 16;
            fcc.AddArea(new CellArea { StartRow = 0, StartColumn = 0, EndRow = 9, EndColumn = 0 });
            fcc[0].Style = style;

            // Starten Sie den Zugriffs-Cache für die bedingte Formatierung
            workbook.StartAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Greifen Sie auf Zellen mit zwischengespeicherter bedingter Formatierung zu
            for (int i = 0; i < 10; i++)
            {
                Cell cell = cells[i, 0];
                Console.WriteLine($"Cell {cell.Name}: Value={cell.StringValue}, FontSize={cell.GetDisplayStyle().Font.Size}");
            }

            // Den Zugriffscache schließen
            workbook.CloseAccessCache(AccessCacheOptions.ConditionalFormatting);

            // Speichere die Arbeitsmappe
            workbook.Save("output.xlsx");
        }
    }
}
```

### Siehe auch

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


