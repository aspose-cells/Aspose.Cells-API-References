---
title: "PageSetup.GetEvenHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup metod. Hämtar ett skript som formaterar den jämna sidhuvudet i en Excel-fil"
type: docs
url: /sv/net/aspose.cells/pagesetup/getevenheader/
---
## PageSetup.GetEvenHeader method

Hämtar ett skript som formaterar jämnt sidhuvud i en Excel-fil.

```csharp
public string GetEvenHeader(int section)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetEvenHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Aktivera olika udda och jämna sidhuvuden/sidfötter
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.IsHFDiffOddEven = true;
            
            // Ställ in jämnt sidhuvud
            pageSetup.SetEvenHeader(0, "&CEven Page Header Center");
            pageSetup.SetEvenHeader(1, "&LEven Page Header Left");
            pageSetup.SetEvenHeader(2, "&REven Page Header Right");
            
            // Hämta och skriv ut jämna sidhuvuden
            Console.WriteLine("Even Header Center: " + pageSetup.GetEvenHeader(0));
            Console.WriteLine("Even Header Left: " + pageSetup.GetEvenHeader(1));
            Console.WriteLine("Even Header Right: " + pageSetup.GetEvenHeader(2));
            
            // Spara arbetsboken
            workbook.Save("PageSetup_GetEvenHeaderDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


