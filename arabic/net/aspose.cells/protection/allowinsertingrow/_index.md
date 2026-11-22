---
title: "Protection.AllowInsertingRow"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Protection. تمثل ما إذا كان إدراج الصفوف مسموحًا به في ورقة عمل محمية"
type: docs
url: /ar/net/aspose.cells/protection/allowinsertingrow/
---
## Protection.AllowInsertingRow property

يمثل ما إذا كان إدراج الصفوف مسموحًا به في ورقة عمل محمية.

```csharp
public bool AllowInsertingRow { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ProtectionPropertyAllowInsertingRowDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى إعدادات الحماية
            Protection protection = worksheet.Protection;

            // تمكين إدراج الصفوف أثناء الحماية
            protection.AllowInsertingRow = true;
            protection.Password = "password123";
            worksheet.Protect(ProtectionType.All);

            // حاول إدراج صف (يجب أن يعمل لأن AllowInsertingRow صحيح)
            worksheet.Cells.InsertRow(0);

            // احفظ المصنف
            workbook.Save("AllowInsertingRowDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [Protection](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


