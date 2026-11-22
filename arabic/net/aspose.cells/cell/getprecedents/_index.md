---
title: "Cell.GetPrecedents"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Cell. تحصل على جميع المراجع التي تظهر في صيغة هذه الخلية"
type: docs
url: /ar/net/aspose.cells/cell/getprecedents/
---
## Cell.GetPrecedents method

يحصل على جميع المراجع التي تظهر في صيغة هذه الخلية.

```csharp
public ReferredAreaCollection GetPrecedents()
```

### قيمة الإرجاع

مجموعة جميع المراجع التي تظهر في صيغة هذه الخلية.

### ملاحظات

يرجع null إذا لم تكن هذه خلية صيغة. سيتم إرجاع جميع المراجع التي تظهر في صيغة هذه الخلية بغض النظر عما إذا كانت مُشارًا إليها أم لا أثناء الحساب. على سبيل المثال، على الرغم من أن الخلية A2 في الصيغة "=IF(TRUE,A1,A2)" لا تُستخدم أثناء الحساب، إلا أنها لا تزال تُعتبر من مراجع الصيغة. للحصول على تلك المراجع التي تؤثر على الحساب فقط، يرجى استخدام [`GetPrecedentsInCalculation`](../getprecedentsincalculation/).

### أمثلة

```csharp
using System;
using System.Text;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellMethodGetPrecedentsDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Cells cells = workbook.Worksheets[0].Cells;
            
            // تعيين صيغة مع المراجع السابقة
            cells["A1"].Formula = "=B1+SUM(B1:B10)+[Book1.xls]Sheet1!A1";
            
            // احصل على جميع المراجع السابقة
            ReferredAreaCollection areas = cells["A1"].GetPrecedents();
            
            // عرض كل مرجع سابق
            foreach (ReferredArea area in areas)
            {
                StringBuilder sb = new StringBuilder();
                if (area.IsExternalLink)
                {
                    sb.Append($"[{area.ExternalFileName}]");
                }
                sb.Append($"{area.SheetName}!");
                sb.Append(CellsHelper.CellIndexToName(area.StartRow, area.StartColumn));
                if (area.IsArea)
                {
                    sb.Append($":{CellsHelper.CellIndexToName(area.EndRow, area.EndColumn)}");
                }
                Console.WriteLine(sb.ToString());
            }
        }
    }
}
```

### انظر أيضًا

* class [ReferredAreaCollection](../../referredareacollection/)
* class [Cell](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


