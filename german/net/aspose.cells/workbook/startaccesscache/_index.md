---
title: "Workbook.StartAccessCache"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "Workbook-Methode. Startet die Sitzung, die Caches zum Zugriff auf Daten verwendet"
type: docs
url: /de/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Startet die Sitzung, die Caches zum Zugriff auf Daten verwendet.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| opts | AccessCacheOptions | Optionen für den Datenzugriff |

### Hinweise

Wenn der Cache des angegebenen Datenzugriffs erfordert, dass einige Datenmodelle im Arbeitsblatt "schreibgeschützt" sind, dann werden die entsprechenden Datenmodelle in jedem Arbeitsblatt dieses Workbooks als "schreibgeschützt" betrachtet und der Benutzer sollte keines davon ändern. Nach Abschluss des Datenzugriffs sollte [`CloseAccessCache`](../closeaccesscache/) mit denselben Optionen aufgerufen werden, um alle Caches zu leeren und den normalen Zugriffsmodus wiederherzustellen.

### Beispiele

```csharp
using System;
using System.Drawing;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookMethodStartAccessCacheWithAccessCacheOptionsDemo
    {
        public static void Run()
        {
            // Erstelle eine Arbeitsmappe
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Bedingte Formatierung hinzufügen
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            int index = cfc.Add();
            cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            
            // Setze Stil für bedingte Formatierung
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            
            // Füge einige eingebettete Bilder hinzu
            Cells cells = sheet.Cells;
            byte[] img1 = File.ReadAllBytes("1.png");
            byte[] img2 = File.ReadAllBytes("2.png");
            cells[0, 0].EmbeddedImage = img1;
            cells[2, 0].EmbeddedImage = img2;
            cells[4, 0].EmbeddedImage = img1;

            // Zugriffscache starten für bessere Leistung
            wb.StartAccessCache(AccessCacheOptions.All);
            
            // Greife auf Zellstile zu (wird dank Caching schneller)
            Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
            
            // Schließe den Cache, wenn er fertig ist
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
    }
}
```

### Siehe auch

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


