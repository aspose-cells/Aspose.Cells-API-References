---
title: "WorkbookSettings.SmartTagOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل على خيارات العلامة الذكية"
type: docs
url: /ar/net/aspose.cells/workbooksettings/smarttagoptions/
---
## WorkbookSettings.SmartTagOptions property

يحصل على خيارات العلامة الذكية.

```csharp
public SmartTagOptions SmartTagOptions { get; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertySmartTagOptionsDemo
    {
        public static void Run()
        {
            try
            {
                // إنشاء دفتر عمل جديد
                Workbook workbook = new Workbook();

                // الوصول إلى إعدادات دفتر العمل
                WorkbookSettings settings = workbook.Settings;

                // اقرأ خاصية SmartTagOptions
                var smartTagOptions = settings.SmartTagOptions;

                // اعرض معلومات حول كائن SmartTagOptions
                Console.WriteLine("SmartTagOptions instance type: " + smartTagOptions.GetType().FullName);

                // اختياريًا، يمكنك فحص الحالة الافتراضية عبر ToString()
                Console.WriteLine("SmartTagOptions details: " + smartTagOptions.ToString());

                // احفظ المصنف (سيحتوي الملف على الإعدادات الافتراضية)
                workbook.Save("SmartTagOptionsDemo.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine($"Error: {ex.Message}");
            }
        }
    }
}
```

### انظر أيضًا

* class [SmartTagOptions](../../../aspose.cells.markup/smarttagoptions/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


