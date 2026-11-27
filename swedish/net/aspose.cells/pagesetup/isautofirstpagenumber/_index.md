---
title: "PageSetup.IsAutoFirstPageNumber"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger om det första sidnumret tilldelas automatiskt"
type: docs
url: /sv/net/aspose.cells/pagesetup/isautofirstpagenumber/
---
## PageSetup.IsAutoFirstPageNumber property

Indikerar om det första sidnumret tilldelas automatiskt.

```csharp
public bool IsAutoFirstPageNumber { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyIsAutoFirstPageNumberDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in sidinställningsegenskaper
            worksheet.PageSetup.IsAutoFirstPageNumber = true;
            Console.WriteLine("Auto First Page Number (Worksheet 1): " + worksheet.PageSetup.IsAutoFirstPageNumber);

            // Lägg till ett andra kalkylblad
            worksheet = workbook.Worksheets.Add("Sheet2");
            worksheet.PageSetup.IsAutoFirstPageNumber = false;
            worksheet.PageSetup.FirstPageNumber = 3;
            Console.WriteLine("Auto First Page Number (Worksheet 2): " + worksheet.PageSetup.IsAutoFirstPageNumber);
            Console.WriteLine("First Page Number (Worksheet 2): " + worksheet.PageSetup.FirstPageNumber);

            // Spara arbetsboken
            workbook.Save("PageSetup_IsAutoFirstPageNumber_Example.xlsx", SaveFormat.Xlsx);
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


