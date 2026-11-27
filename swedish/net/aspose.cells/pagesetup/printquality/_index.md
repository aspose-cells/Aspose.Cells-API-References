---
title: "PageSetup.PrintQuality"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger utskriftskvaliteten"
type: docs
url: /sv/net/aspose.cells/pagesetup/printquality/
---
## PageSetup.PrintQuality property

Anger utskriftskvaliteten.

```csharp
public int PrintQuality { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintQualityDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in utskriftskvalitet till 144 dpi
            worksheet.PageSetup.PrintQuality = 144;
            
            // Skriv ut den aktuella utskriftskvalitetsinställningen
            Console.WriteLine("Print Quality: " + worksheet.PageSetup.PrintQuality);
            
            // Spara arbetsboken
            workbook.Save("PrintQualityDemo.xls");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


