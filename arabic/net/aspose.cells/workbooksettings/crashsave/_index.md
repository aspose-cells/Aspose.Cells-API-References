---
title: "WorkbookSettings.CrashSave"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تشير إلى ما إذا كان التطبيق قد حفظ ملف المصنف آخر مرة بعد حدوث عطل"
type: docs
url: /ar/net/aspose.cells/workbooksettings/crashsave/
---
## WorkbookSettings.CrashSave property

يشير إلى ما إذا كان التطبيق قد حفظ ملف المصنف آخر مرة بعد تعطل.

```csharp
public bool CrashSave { get; set; }
```

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyCrashSaveDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            sheet.Cells["A1"].PutValue("CrashSave Demo");
            sheet.Cells["A2"].PutValue(DateTime.Now);

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // إظهار خاصية CrashSave
            settings.CrashSave = true;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // حفظ مع تمكين حفظ التعطل
            workbook.Save("CrashSaveEnabled.xlsx");

            // تعطيل حفظ التعطل
            settings.CrashSave = false;
            Console.WriteLine($"CrashSave enabled: {settings.CrashSave}");

            // حفظ مع تعطيل حفظ التعطل
            workbook.Save("CrashSaveDisabled.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


