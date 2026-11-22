---
title: "Protection.AllowInsertingColumn"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان إدراج الأعمدة مسموحًا به في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowinsertingcolumn/
---
## Protection.AllowInsertingColumn property

يمثل ما إذا كان إدراج الأعمدة مسموحًا به في ورقة عمل محمية.

```csharp
public bool AllowInsertingColumn { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingColumnDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // احصل على إعدادات الحماية
            Protection protection = worksheet.Protection;

            // عيّن AllowInsertingColumn إلى true
            protection.AllowInsertingColumn = true;

            // تحقق من الإعداد
            Console.WriteLine("AllowInsertingColumn is set to: " + protection.AllowInsertingColumn);

            // احمِ ورقة العمل بكلمة مرور (باستخدام طريقة Workbook.Protect)
            workbook.Protect(ProtectionType.All, "password123");
            protection.AllowInsertingColumn = true; // Explicitly set again to demonstrate

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


