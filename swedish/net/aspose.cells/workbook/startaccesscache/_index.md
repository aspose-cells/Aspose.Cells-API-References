---
title: "Workbook.StartAccessCache"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Workbook-metod. Startar sessionen som använder cache för att komma åt data"
type: docs
url: /sv/net/aspose.cells/workbook/startaccesscache/
---
## Workbook.StartAccessCache method

Startar sessionen som använder cache för att komma åt data.

```csharp
public void StartAccessCache(AccessCacheOptions opts)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| opts | AccessCacheOptions | alternativ för dataåtkomst |

### Anmärkningar

Om cachen för den angivna dataåtkomsten kräver att vissa datamodeller i kalkylbladet är "read-only", kommer motsvarande datamodeller i varje kalkylblad i den här arbetsboken att behandlas som "read-only" och användaren bör inte ändra någon av dem. Efter att åtkomsten till data är avslutad, [`CloseAccessCache`](../closeaccesscache/) bör anropas med samma alternativ för att rensa alla cachar och återställa normalt åtkomstläge.

### Exempel

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
            // Skapa en arbetsbok
            Workbook wb = new Workbook();
            Worksheet sheet = wb.Worksheets[0];
            
            // Lägg till villkorsstyrd formatering
            ConditionalFormattingCollection cfc = sheet.ConditionalFormattings;
            int index = cfc.Add();
            cfc[index].Add(CellArea.CreateCellArea(0, 0, 5, 0),
                FormatConditionType.DuplicateValues, OperatorType.None, null, null);
            
            // Ställ in stil för villkorsstyrd formatering
            Style style = cfc[0][0].Style;
            style.ForegroundColor = Color.Red;
            style.Pattern = BackgroundType.Solid;
            
            // Lägg till några inbäddade bilder
            Cells cells = sheet.Cells;
            byte[] img1 = File.ReadAllBytes("1.png");
            byte[] img2 = File.ReadAllBytes("2.png");
            cells[0, 0].EmbeddedImage = img1;
            cells[2, 0].EmbeddedImage = img2;
            cells[4, 0].EmbeddedImage = img1;

            // Starta åtkomstcache för bättre prestanda
            wb.StartAccessCache(AccessCacheOptions.All);
            
            // Åtkomst till cellstilar (kommer att bli snabbare på grund av cachning)
            Console.WriteLine("A1 Pattern: " + cells[0, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A3 Pattern: " + cells[2, 0].GetDisplayStyle().Pattern);
            Console.WriteLine("A5 Pattern: " + cells[4, 0].GetDisplayStyle().Pattern);
            
            // Stäng cachen när du är klar
            wb.CloseAccessCache(AccessCacheOptions.All);
        }
    }
}
```

### Se även

* enum [AccessCacheOptions](../../accesscacheoptions/)
* class [Workbook](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


