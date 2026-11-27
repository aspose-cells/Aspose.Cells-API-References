---
title: "PageSetup.CenterVertically"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger om bladet skrivs ut centrerat vertikalt"
type: docs
url: /sv/net/aspose.cells/pagesetup/centervertically/
---
## PageSetup.CenterVertically property

Representerar om bladet skrivs ut centrerat vertikalt.

```csharp
public bool CenterVertically { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterVerticallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // Kom åt PageSetup och sätt CenterVertically
            PageSetup pageSetup = worksheet.PageSetup;
            pageSetup.CenterVertically = true;
            
            // Lägg till lite exempeldata för att visualisera effekten
            worksheet.Cells["A1"].PutValue("This worksheet content will be centered vertically when printed");
            worksheet.Cells["A2"].PutValue("CenterVertically = true");
            
            // Spara arbetsboken
            workbook.Save("PageSetup_CenterVertically.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


