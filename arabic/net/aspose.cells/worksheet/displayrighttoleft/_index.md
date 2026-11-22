---
title: "Worksheet.DisplayRightToLeft"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تشير إلى ما إذا كان ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/worksheet/displayrighttoleft/
---
## Worksheet.DisplayRightToLeft property

يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false.

```csharp
public bool DisplayRightToLeft { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyDisplayRightToLeftDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // عيّن العرض من اليمين إلى اليسار
            worksheet.DisplayRightToLeft = true;
            
            // احفظ المصنف
            workbook.Save("output.ods");
            
            // أعد تحميل المصنف للتحقق من الإعداد
            Workbook loadedWorkbook = new Workbook("output.ods");
            Worksheet loadedWorksheet = loadedWorkbook.Worksheets[0];
            
            Console.WriteLine("DisplayRightToLeft: " + loadedWorksheet.DisplayRightToLeft);
        }
    }
}
```

### انظر أيضًا

* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


