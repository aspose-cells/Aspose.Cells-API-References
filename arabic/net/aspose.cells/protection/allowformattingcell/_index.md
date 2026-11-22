---
title: "Protection.AllowFormattingCell"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان تنسيق الخلايا مسموحًا به في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowformattingcell/
---
## Protection.AllowFormattingCell property

يمثل ما إذا كان تنسيق الخلايا مسموحًا به في ورقة عمل محمية.

```csharp
public bool AllowFormattingCell { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingCellDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تمكين حماية ورقة العمل
            Protection protection = worksheet.Protection;
            
            // ضبط خصائص حماية متعددة باستخدام علم
            int flag = 0x40; // Only AllowFormattingCell flag is set
            protection.AllowFormattingCell = (flag & 0x40) != 0;

            // تحقق من الإعداد
            Console.WriteLine("AllowFormattingCell is set to: " + protection.AllowFormattingCell);

            // احفظ المصنف
            workbook.Save("ProtectionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


