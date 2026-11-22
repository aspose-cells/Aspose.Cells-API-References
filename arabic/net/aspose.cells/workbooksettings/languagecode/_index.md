---
title: "WorkbookSettings.LanguageCode"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية WorkbookSettings. تحصل أو تعين لغة واجهة المستخدم لإصدار المصنف بناءً على CountryCode الذي حفظ الملف"
type: docs
url: /ar/net/aspose.cells/workbooksettings/languagecode/
---
## WorkbookSettings.LanguageCode property

يحصل أو يضبط لغة واجهة المستخدم لإصدار Workbook بناءً على رمز البلد (CountryCode) الذي حفظ الملف.

```csharp
public CountryCode LanguageCode { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class WorkbookSettingsPropertyLanguageCodeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // تعيين رمز اللغة إلى الألمانية (Germany)
            settings.LanguageCode = CountryCode.Germany;

            // عرض رمز اللغة الحالي
            Console.WriteLine("Current Language Code: " + settings.LanguageCode);

            // تغيير رمز اللغة إلى الفرنسية (France)
            settings.LanguageCode = CountryCode.France;
            Console.WriteLine("Updated Language Code: " + settings.LanguageCode);

            // احفظ المصنف
            workbook.Save("WorkbookSettings_LanguageCodeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [CountryCode](../../countrycode/)
* class [WorkbookSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


