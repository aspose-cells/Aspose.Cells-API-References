---
title: "ReferredArea.EndRow"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ReferredArea özelliği. Alanın son satırı"
type: docs
url: /tr/net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

Alanının son satırı.

```csharp
public int EndRow { get; }
```

### Örnekler

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
            
            // Birden fazla referans içeren formülü ayarlayın
            cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
            
            // Tüm önceki alanları alın
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // Her referansı işleyin
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                
                // Aralık referansları için EndRow kullanımını gösterin
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

### Ayrıca Bakınız

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


