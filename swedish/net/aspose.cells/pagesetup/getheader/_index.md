---
title: "PageSetup.GetHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Hämtar ett skript som formaterar rubriken i en Excel-fil"
type: docs
url: /sv/net/aspose.cells/pagesetup/getheader/
---
## PageSetup.GetHeader method

Hämtar ett skript som formaterar sidhuvud i en Excel-fil.

```csharp
public string GetHeader(int section)
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
    public class PageSetupMethodGetHeaderWithInt32Demo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in rubriken för sektion 2
            worksheet.PageSetup.SetHeader(2, "&8Report ID: TEST01\n你好Public");
            
            // Hämta och skriv ut rubriken för sektion 2
            string header = worksheet.PageSetup.GetHeader(2);
            Console.WriteLine("Header for section 2: " + header);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


