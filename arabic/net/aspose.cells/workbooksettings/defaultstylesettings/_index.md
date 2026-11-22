---
title: "WorkbookSettings.DefaultStyleSettings"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. الحصول على الإعدادات للقيم الافتراضية للخصائص المتعلقة بالنمط لهذا المصنف"
type: docs
url: /ar/net/aspose.cells/workbooksettings/defaultstylesettings/
---
## WorkbookSettings.DefaultStyleSettings property

يحصل على الإعدادات للقيم الافتراضية للخصائص المتعلقة بالنمط لهذا المصنف.

```csharp
public DefaultStyleSettings DefaultStyleSettings { get; }
```

### أمثلة

```csharp
using System;
using System.Globalization;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyDefaultStyleSettingsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات النمط الافتراضية
            DefaultStyleSettings styleSettings = workbook.Settings.DefaultStyleSettings;

            // تعيين تفضيل تنسيق الأرقام المدمج
            styleSettings.BuiltInPreference = true;

            // تعيين الثقافة لتنسيق الأرقام
            workbook.Settings.CultureInfo = new CultureInfo("en-US");

            // الوصول إلى الخلايا وتطبيق التنسيق
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;

            // تعيين القيم والأنماط
            cells["A1"].PutValue(1234.56);
            cells["A1"].GetStyle().Number = 4; // Currency format

            cells["B1"].PutValue(0.456);
            cells["B1"].GetStyle().Number = 2; // Percentage format

            cells["C1"].PutValue(DateTime.Now);
            cells["C1"].GetStyle().Number = 22; // Short date format

            // احفظ المصنف
            workbook.Save("DefaultStyleSettingsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [DefaultStyleSettings](../../defaultstylesettings/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


