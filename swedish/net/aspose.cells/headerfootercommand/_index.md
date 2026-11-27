---
title: "Klass HeaderFooterCommand"
second_title: "Aspose.Cells för .NET API‑referens"
description: "Aspose.Cells.HeaderFooterCommand-klass. Representerar kommandot för sidhuvud/sidfot"
type: docs
url: /sv/net/aspose.cells/headerfootercommand/
---
## HeaderFooterCommand class

Representerar kommandot för sidhuvud/sidfot

```csharp
public class HeaderFooterCommand
```

## Egenskaper

| Namn | Beskrivning |
| --- | --- |
| [Font](../../aspose.cells/headerfootercommand/font/) { get; } | Hämtar teckensnittet för kommandots värde. |
| [Text](../../aspose.cells/headerfootercommand/text/) { get; } | Hämtar texten för kommandot. |
| [Type](../../aspose.cells/headerfootercommand/type/) { get; } | Hämtar header/footer-kommandotypen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassHeaderFooterCommandDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Åtkomst till PageSetup och ställ in header med kommandon
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.SetHeader(1, "&D&\"Arial\"sdfsdfsdfsdf");
            
            // Hämta header-kommandon
            HeaderFooterCommand[] commands = pageSetup.GetCommands(pageSetup.GetHeader(1));
            
            // Visa kommandotyper och text
            Console.WriteLine("Command 1 Type: " + commands[0].Type);
            Console.WriteLine("Command 2 Type: " + commands[1].Type);
            Console.WriteLine("Command 2 Text: " + commands[1].Text);
        }
    }
}
```

### Se även

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


