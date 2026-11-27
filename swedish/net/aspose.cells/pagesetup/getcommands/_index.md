---
title: "PageSetup.GetCommands"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Hämtar alla kommandon för sidhuvud eller sidfot."
type: docs
url: /sv/net/aspose.cells/pagesetup/getcommands/
---
## PageSetup.GetCommands method

Hämtar alla kommandon för sidhuvud eller sidfot.

```csharp
public HeaderFooterCommand[] GetCommands(string headerFooterScript)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| headerFooterScript | String | Sidhuvud/sidfot-skriptet. |

### Returvärde

Returnerar alla kommandon för sidhuvud eller sidfot.

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodGetCommandsWithStringDemo
    {
        public static void Run()
        {
            // Skapa en arbetsbok
            Workbook workbook = new Workbook();
            
            // Kom åt första arbetsbladet
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in sidhuvud med kommandon.
            string header = "&D&\"Arial\"&12sdfsdfsdfsdf";
            worksheet.PageSetup.SetHeader(1, header);
            
            // Hämta header-kommandon
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(header);
            
            // Visa kommandotyper och text
            foreach (HeaderFooterCommand cmd in commands)
            {
                Console.WriteLine($"Type: {cmd.Type}, Text: {cmd.Text}");
            }
        }
    }
}
```

### Se även

* class [HeaderFooterCommand](../../headerfootercommand/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


