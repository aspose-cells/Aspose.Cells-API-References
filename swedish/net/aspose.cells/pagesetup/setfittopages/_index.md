---
title: "PageSetup.SetFitToPages"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup metod. Anger antalet sidor som kalkylbladet skalas till när det skrivs ut"
type: docs
url: /sv/net/aspose.cells/pagesetup/setfittopages/
---
## PageSetup.SetFitToPages method

Ställer in antalet sidor som kalkylbladet skalas till när det skrivs ut.

```csharp
public void SetFitToPages(int wide, int tall)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| bred | Int32 | Sidor breda. |
| hög | Int32 | Sidor höga. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetFitToPagesWithInt32Int32Demo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt den första kalkylbladets PageSetup
            PageSetup setup = workbook.Worksheets[0].PageSetup;
            
            // Ställ in inställningarna för anpassning till sidor
            setup.SetFitToPages(2, 3);
            
            // Verifiera och skriv ut inställningarna
            Console.WriteLine("IsPercentScale: " + setup.IsPercentScale);
            Console.WriteLine("FitToPagesWide: " + setup.FitToPagesWide);
            Console.WriteLine("FitToPagesTall: " + setup.FitToPagesTall);
            
            // Spara arbetsboken
            workbook.Save("output.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


