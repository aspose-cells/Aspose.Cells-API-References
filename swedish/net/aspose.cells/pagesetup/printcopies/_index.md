---
title: "PageSetup.PrintCopies"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Hämtar och anger antal kopior att skriva ut"
type: docs
url: /sv/net/aspose.cells/pagesetup/printcopies/
---
## PageSetup.PrintCopies property

Hämtar och anger antal kopior att skriva ut.

```csharp
public int PrintCopies { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintCopiesDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in antalet utskriftskopior till 3
            worksheet.PageSetup.PrintCopies = 3;
            
            // Visa den aktuella inställningen för utskriftskopior
            Console.WriteLine("Print Copies: " + worksheet.PageSetup.PrintCopies);
            
            // Spara arbetsboken
            workbook.Save("PageSetup_PrintCopies_Output.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


