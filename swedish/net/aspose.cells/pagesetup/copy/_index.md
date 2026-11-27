---
title: "PageSetup.Copy"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Kopierar inställningarna för sidinställningen"
type: docs
url: /sv/net/aspose.cells/pagesetup/copy/
---
## PageSetup.Copy method

Kopierar inställningarna för sidlayout.

```csharp
public void Copy(PageSetup source, CopyOptions copyOptions)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| källa | PageSetup | Källan. |
| copyOptions | CopyOptions | Kopieringsalternativen. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodCopyWithPageSetupCopyOptionsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add();
            
            // Ställ in PageSetup-egenskaper för det första kalkylbladet
            workbook.Worksheets[0].PageSetup.PaperSize = PaperSizeType.PaperA3;
            
            // Kopiera PageSetup från första kalkylbladet till andra kalkylbladet med CopyOptions
            workbook.Worksheets[1].PageSetup.Copy(workbook.Worksheets[0].PageSetup, new CopyOptions());
            
            Console.WriteLine("Paper size of second worksheet: " + workbook.Worksheets[1].PageSetup.PaperSize);
        }
    }
}
```

### Se även

* class [CopyOptions](../../copyoptions/)
* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


