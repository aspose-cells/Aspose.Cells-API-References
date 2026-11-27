---
title: "ReferredArea.EndRow"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ReferredArea-egenskap. Slutrad i området"
type: docs
url: /sv/net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

Slutraden för området.

```csharp
public int EndRow { get; }
```

### Exempel

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ReferredAreaPropertyEndRowDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // Ange formel med flera referenser
            cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
            
            // Hämta alla föregående områden
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Bearbeta varje referens
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                
                // Demonstrera användning av EndRow för områdesreferenser
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                
                Console.WriteLine(sb.ToString());
            }
            
            workbook.Save("ReferredAreaExample.xlsx");
        }
    }
}
```

### Se även

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


