---
title: "PageSetup.CenterHorizontally"
second_title: "Aspose.Cells för .NET API‑referens"
description: "PageSetup-egenskap. Anger om bladet skrivs ut centrerat horisontellt"
type: docs
url: /sv/net/aspose.cells/pagesetup/centerhorizontally/
---
## PageSetup.CenterHorizontally property

Representerar om bladet skrivs ut centrerat horisontellt.

```csharp
public bool CenterHorizontally { get; set; }
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class PageSetupPropertyCenterHorizontallyDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Fyll i lite exempeldata
            worksheet.Cells["A1"].PutValue("Sample Data");
            for (int i = 1; i <= 5; i++)
            {
                worksheet.Cells["A" + (i + 1)].PutValue("Item " + i);
                worksheet.Cells["B" + (i + 1)].PutValue(i * 100);
            }

            PageSetup pageSetup = worksheet.PageSetup;
            
            // Demonstrera egenskapen CenterHorizontally
            pageSetup.CenterHorizontally = true;
            pageSetup.PrintArea = "A1:B6";

            workbook.Save("CenterHorizontallyDemo.xlsx");
        }
    }
}
```

### Se även

* class [PageSetup](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


