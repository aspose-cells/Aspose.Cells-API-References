---
title: "PageSetup.BlackAndWhite"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup egenskap. Representerar om element i dokumentet kommer att skrivas ut i svartvitt"
type: docs
url: /sv/net/aspose.cells/pagesetup/blackandwhite/
---
## PageSetup.BlackAndWhite property

Representerar om element i dokumentet kommer att skrivas ut i svartvitt.

```csharp
public bool BlackAndWhite { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyBlackAndWhiteDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Hämta PageSetup-objektet
            PageSetup pageSetup = worksheet.PageSetup;

            // Ställ in BlackAndWhite property till sant
            pageSetup.BlackAndWhite = true;
            Console.WriteLine("BlackAndWhite set to: " + pageSetup.BlackAndWhite);

            // Ändra BlackAndWhite property till falskt
            pageSetup.BlackAndWhite = false;
            Console.WriteLine("BlackAndWhite changed to: " + pageSetup.BlackAndWhite);

            // Spara arbetsboken
            workbook.Save("PageSetupBlackAndWhiteDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


