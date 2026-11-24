---
title: "PageSetup.PaperSize"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt die Papiergröße an"
type: docs
url: /de/net/aspose.cells/pagesetup/papersize/
---
## PageSetup.PaperSize property

Stellt die Größe des Papiers dar.

```csharp
public PaperSizeType PaperSize { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyPaperSizeDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Setzen Sie die Papiergröße auf Umschlag B6
            sheet.PageSetup.PaperSize = PaperSizeType.PaperEnvelopeB6;

            // Geben Sie die aktuelle Papiergröße aus
            Console.WriteLine("Current paper size: " + sheet.PageSetup.PaperSize);

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetup_PaperSizeDemo.xlsx");
        }
    }
}
```

### Siehe auch

* enum [PaperSizeType](../../papersizetype/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


