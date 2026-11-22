---
title: "Worksheet.Protection"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية Worksheet. تمثل الأنواع المختلفة لخيارات الحماية المتاحة لورقة العمل. تدعم خيارات الحماية المتقدمة في ExcelXP والإصدارات الأحدث."
type: docs
url: /ar/net/aspose.cells/worksheet/protection/
---
## Worksheet.Protection property

يمثل الأنواع المختلفة لخيارات الحماية المتاحة لورقة العمل. يدعم خيارات الحماية المتقدمة في ExcelXP والإصدارات الأحدث.

```csharp
public Protection Protection { get; }
```

### ملاحظات

يمكن لهذه الخاصية حماية ورقة العمل في جميع إصدارات ملف Excel وتدعم خيارات الحماية المتقدمة في ExcelXP والإصدارات الأحدث.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorksheetPropertyProtectionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // الوصول إلى خصائص الحماية
            Protection protection = sheet.Protection;
            
            // تعيين خصائص الحماية
            protection.AllowEditingObject = false;
            protection.AllowEditingScenario = false;
            
            // حماية ورقة العمل (باستخدام طريقة Protect بدلاً من ضبط IsProtectedWithPassword مباشرةً)
            sheet.Protect(ProtectionType.All, "password123", null);

            // احفظ المصنف
            workbook.Save("WorksheetProtectionDemo.xlsx");

            // تحقق من إعدادات الحماية
            Console.WriteLine("AllowEditingObject: " + protection.AllowEditingObject);
            Console.WriteLine("AllowEditingScenario: " + protection.AllowEditingScenario);
        }
    }
}
```

### انظر أيضًا

* class [Protection](../../protection/)
* class [Worksheet](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


