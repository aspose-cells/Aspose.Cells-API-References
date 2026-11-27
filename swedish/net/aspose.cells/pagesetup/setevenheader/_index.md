---
title: "PageSetup.SetEvenHeader"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-metod. Ställer in ett skript som formaterar den jämna sidhuvudet i en Excel-fil. Påverkar endast i Excel 2007 när IsHFDiffOddEven är sant"
type: docs
url: /sv/net/aspose.cells/pagesetup/setevenheader/
---
## PageSetup.SetEvenHeader method

Ställer in ett skript som formaterar den jämna sidhuvudet i en Excel-fil. Endast effekt i Excel 2007 när IsHFDiffOddEven är sant.

```csharp
public void SetEvenHeader(int section, string headerScript)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sektion | Int32 | 0: Vänster sektion, 1: Centrerad sektion, 2: Höger sektion. |
| headerScript | String | Rubrikformatskript. |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupMethodSetEvenHeaderWithInt32StringDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;

            // Aktivera olika sidhuvuden/sidfötter för udda och jämna sidor
            pageSetup.IsHFDiffOddEven = true;

            // Ställ in jämnt sidhuvud med sektionsindex och text
            pageSetup.SetEvenHeader(1, "Even Page Header - Center Section");
            pageSetup.SetEvenHeader(0, "Even Page Header - Left Section");
            pageSetup.SetEvenHeader(2, "Even Page Header - Right Section");

            // Spara arbetsboken
            workbook.Save("PageSetup_SetEvenHeaderExample.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


