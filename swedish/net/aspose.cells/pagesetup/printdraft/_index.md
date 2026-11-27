---
title: "PageSetup.PrintDraft"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger om bladet ska skrivas ut utan grafik"
type: docs
url: /sv/net/aspose.cells/pagesetup/printdraft/
---
## PageSetup.PrintDraft property

Anger om bladet ska skrivas ut utan grafik.

```csharp
public bool PrintDraft { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintDraftDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Kom åt PageSetup-objektet
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in PrintDraft-egenskapen till true
            pageSetup.PrintDraft = true;
            Console.WriteLine("PrintDraft set to: " + pageSetup.PrintDraft);

            // Ändra PrintDraft-egenskapen till false
            pageSetup.PrintDraft = false;
            Console.WriteLine("PrintDraft changed to: " + pageSetup.PrintDraft);

            // Spara arbetsboken
            workbook.Save("PageSetup_PrintDraft_Example.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


