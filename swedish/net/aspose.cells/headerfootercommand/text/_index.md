---
title: "HeaderFooterCommand.Text"
second_title: "Aspose.Cells för .NET API‑referens"
description: "HeaderFooterCommand‑egenskap. Hämtar kommandots text"
type: docs
url: /sv/net/aspose.cells/headerfootercommand/text/
---
## HeaderFooterCommand.Text property

Hämtar texten för kommandot.

```csharp
public string Text { get; }
```

### Anmärkningar

Endast giltig för HeaderFooterCommandType.Text.

### Exempel

```csharp
using System;
using Aspose.Cells;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class HeaderFooterCommandPropertyTextDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Ställ in rubrik med textkommando
            worksheet.PageSetup.SetHeader(1, "&\"Arial\"&12&KFF0000Sample Text Header");
            
            // Hämta header-kommandon
            HeaderFooterCommand[] commands = worksheet.PageSetup.GetCommands(worksheet.PageSetup.GetHeader(1));
            
            // Visa information om textkommando
            foreach (HeaderFooterCommand cmd in commands)
            {
                if (cmd.Type == HeaderFooterCommandType.Text)
                {
                    Console.WriteLine("Text command found:");
                    Console.WriteLine("Text: " + cmd.Text);
                    Console.WriteLine("Font: " + cmd.Font);
                    Console.WriteLine("Color: " + ColorTranslator.ToHtml(cmd.Font.Color));
                }
            }
            
            // Spara arbetsboken
            workbook.Save("HeaderFooterTextDemo.xlsx");
        }
    }
}
```

### Se även

* class [HeaderFooterCommand](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


