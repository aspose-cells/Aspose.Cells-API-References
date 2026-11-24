---
title: "PageSetup.BlackAndWhite"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "PageSetup-Eigenschaft. Gibt an, ob Elemente des Dokuments in Schwarz‑Weiß gedruckt werden."
type: docs
url: /de/net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

Gibt an, ob Elemente des Dokuments in Schwarzweiß gedruckt werden.

```csharp
public bool BlackAndWhite { get; set; }
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBlackAndWhiteDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Das PageSetup-Objekt abrufen
            PageSetup pageSetup = worksheet.PageSetup;

            // Setze die BlackAndWhite‑Eigenschaft auf true
            pageSetup.BlackAndWhite = true;
            Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);

            // Ändere die BlackAndWhite‑Eigenschaft auf false
            pageSetup.BlackAndWhite = false;
            Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);

            // Speichere die Arbeitsmappe
            workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
        }
    }
}
```

### Siehe auch

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


