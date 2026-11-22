---
title: "Protection.AllowFormattingRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان تنسيق الصفوف مسموحًا به في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowformattingrow/
---
## Protection.AllowFormattingRow property

يمثل ما إذا كان تنسيق الصفوف مسموحًا به في ورقة عمل محمية.

```csharp
public bool AllowFormattingRow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowFormattingRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // تمكين حماية ورقة العمل
            worksheet.Protect(ProtectionType.All);

            // الوصول إلى إعدادات الحماية
            Protection protection = worksheet.Protection;

            // السماح بتنسيق الصفوف مع الحفاظ على الحمايات الأخرى
            protection.AllowFormattingRow = true;

            // احفظ المصنف
            workbook.Save("Protection_AllowFormattingRow.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


