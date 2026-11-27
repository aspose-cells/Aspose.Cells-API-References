---
title: "HighlightChangesOptions.HighlightChangesOptions"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HighlightChangesOptions‑konstruktorn. Representerar alternativ för att markera revisioner eller ändringar i delade Excel‑filer"
type: docs
url: /sv/net/aspose.cells.revisions/highlightchangesoptions/highlightchangesoptions/
---
## HighlightChangesOptions constructor

Representerar alternativ för att markera revisioner eller ändringar i delade Excel‑filer.

```csharp
public HighlightChangesOptions(bool highlightOnScreen, bool listOnNewSheet)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| highlightOnScreen | Boolean | Indikerar om förändringar markeras på skärmen. |
| listOnNewSheet | Boolean | Indikerar om förändringar listas på ett nytt kalkylblad. |

### Exempel

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Revisions;

namespace AsposeCellsExamples
{
    public class HighlightChangesOptionsMethodCtorWithBooleanBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite exempeldata
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Original Value");
            worksheet.Cells["A2"].PutValue(100);
            
            // Skapa HighlightChangesOptions med booleska parametrar
            HighlightChangesOptions options = new HighlightChangesOptions(true, true);
            
            // Simulera spårning av ändringar (normalt skulle du ha faktiska revisioner)
            Console.WriteLine("HighlightChangesOptions created with:");
            Console.WriteLine($"First parameter (show changes): {true}");
            Console.WriteLine($"Second parameter (changes on new sheet): {true}");
            
            // Spara arbetsboken
            workbook.Save("HighlightChangesDemo.xlsx");
        }
    }
}
```

### Se även

* class [HighlightChangesOptions](../)
* namespace [Aspose.Cells.Revisions](../../../aspose.cells.revisions/)
* assembly [Aspose.Cells](../../../)


