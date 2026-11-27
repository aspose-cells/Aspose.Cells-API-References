---
title: "PageSetup.PrintErrors"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger typen av utskriftsfel som visas"
type: docs
url: /sv/net/aspose.cells/pagesetup/printerrors/
---
## PageSetup.PrintErrors property

Anger vilken typ av utskriftsfel som visas.

```csharp
public PrintErrorsType PrintErrors { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPrintErrorsDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Åtkomst till det första kalkylbladet
            Worksheet sheet = workbook.Worksheets[0];
            
            // Ställ in utskriftsfel att visas som tomt
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsBlank;
            Console.WriteLine("PrintErrors set to: " + sheet.PageSetup.PrintErrors);
            
            // Ändra utskriftsfel att visas som streck
            sheet.PageSetup.PrintErrors = PrintErrorsType.PrintErrorsDash;
            Console.WriteLine("PrintErrors changed to: " + sheet.PageSetup.PrintErrors);
            
            // Spara arbetsboken
            workbook.Save("PrintErrorsDemo.xlsx");
        }
    }
}
```

### Se även

* enum [PrintErrorsType](../../printerrorstype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


