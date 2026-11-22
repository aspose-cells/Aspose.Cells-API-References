---
title: "ReferredArea.EndRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ReferredArea. الصف النهائي للمنطقة"
type: docs
url: /ar/net/aspose.cells/referredarea/endrow/
---
## ReferredArea.EndRow property

صف النهاية للمنطقة.

```csharp
public int EndRow { get; }
```

### أمثلة

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
            
            // عيّن صيغة مع مراجع متعددة
            cells["A1"].Formula = "= B1 + SUM(B1:B10) + [Book1.xls]Sheet1!A1";
            
            // احصل على جميع المناطق السابقة
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // معالجة كل مرجع
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                
                // عرض استخدام EndRow لمراجع النطاق
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

### انظر أيضًا

* class [ReferredArea](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


