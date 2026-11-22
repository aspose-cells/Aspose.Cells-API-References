---
title: "WorkbookSettings.IsMinimized"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تمثل ما إذا كان سيتم فتح جدول البيانات المُنشأ في وضع مصغر"
type: docs
url: /ar/net/aspose.cells/workbooksettings/isminimized/
---
## WorkbookSettings.IsMinimized property

يمثل ما إذا كان الجدول الإلكتروني المُنشأ سيفتح مصغّرًا.

```csharp
public bool IsMinimized { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyIsMinimizedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // عيّن خاصية IsMinimized إلى true
            workbook.Settings.IsMinimized = true;

            // احفظ المصنف
            workbook.Save("IsMinimizedDemo.xlsx");

            // حمّل دفتر العمل المحفوظ للتحقق من الخاصية
            Workbook loadedWorkbook = new Workbook("IsMinimizedDemo.xlsx");

            // أخرج قيمة خاصية IsMinimized
            Console.WriteLine("Workbook IsMinimized property: " + loadedWorkbook.Settings.IsMinimized);
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


