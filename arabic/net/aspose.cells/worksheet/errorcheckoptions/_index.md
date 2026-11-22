---
title: "Worksheet.ErrorCheckOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. يحصل على إعداد فحص الأخطاء المطبق على نطاقات معينة"
type: docs
url: /ar/net/aspose.cells/worksheet/errorcheckoptions/
---
## Worksheet.ErrorCheckOptions property

يحصل على إعداد فحص الأخطاء المطبق على نطاقات معينة.

```csharp
public ErrorCheckOptionCollection ErrorCheckOptions { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyErrorCheckOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // فعّل خيارات فحص الأخطاء
            ErrorCheckOptionCollection options = worksheet.ErrorCheckOptions;
            ErrorCheckOption option = options[0]; // Properly access first option using indexer
            option.SetErrorCheck(ErrorCheckType.TextDate, true);
            option.AddRange(CellArea.CreateCellArea(0, 0, 10, 10));
            
            // احصل على عدد النطاقات للخيار
            int rangeCount = option.GetCountOfRange();
            Console.WriteLine("Number of ranges in ErrorCheckOption: " + rangeCount);
            
            // احفظ المصنف
            workbook.Save("ErrorCheckOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ErrorCheckOptionCollection](../../errorcheckoptioncollection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


