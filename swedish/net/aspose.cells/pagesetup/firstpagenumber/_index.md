---
title: "PageSetup.FirstPageNumber"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Representerar det första sidnumret som kommer att användas när detta blad skrivs ut"
type: docs
url: /sv/net/aspose.cells/pagesetup/firstpagenumber/
---
## PageSetup.FirstPageNumber property

Representerar det första sidnumret som kommer att användas när detta blad skrivs ut.

```csharp
public int FirstPageNumber { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyFirstPageNumberDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in sidinställningsegenskaper
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            
            // Skriv ut resultaten
            Console.WriteLine("IsAutoFirstPageNumber: " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("FirstPageNumber: " + worksheet.PageSetup.FirstPageNumber);
            
            // Spara arbetsboken
            workbook.Save("PageSetupFirstPageNumberDemo.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


