---
title: "HeaderFooterCommand.Type"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HeaderFooterCommand-egenskap. Hämtar header/footer-kommandometypen"
type: docs
url: /sv/net/aspose.cells/headerfootercommand/type/
---
## HeaderFooterCommand.Type property

Hämtar header/footer-kommandotypen.

```csharp
public HeaderFooterCommandType Type { get; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTypeDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in sidhuvud med olika kommandotyper
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(0, "&D&\"Arial\"&12sdfsdfsdfsdf");
            
            // Hämta header-kommandon
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(0));
            
            // Demonstrera användning av Type-egenskapen
            Console.WriteLine("Command 0 Type: " + commands[0].Type); // CurrentDate
            Console.WriteLine("Command 1 Type: " + commands[1].Type); // Text
            Console.WriteLine("Command 1 Text: " + commands[1].Text); // sdfsdfsdfsdf
        }
    }
}
```

### Se även

* enum [HeaderFooterCommandType](../../headerfootercommandtype/)
* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


