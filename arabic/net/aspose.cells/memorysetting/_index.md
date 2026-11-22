---
title: "التعداد MemorySetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.MemorySetting. أوضاع استخدام الذاكرة لنموذج بيانات الخلايا"
type: docs
url: /ar/net/aspose.cells/memorysetting/
---
## MemorySetting enumeration

أنماط استخدام الذاكرة لنموذج بيانات الخلايا.

```csharp
public enum MemorySetting
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Normal | `0` | الوضع الافتراضي لنموذج الخلايا. |
| MemoryPreference | `1` | يفضل أداء الذاكرة. |
| FileCache | `2` | يفضل أداء الذاكرة واستخدام ملف بدلاً من الذاكرة للحفاظ على بيانات الخلايا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class MemorySettingDemo
    {
        public static void MemorySettingExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات دفتر العمل
            WorkbookSettings settings = workbook.Settings;

            // اضبط خيار استخدام الذاكرة إلى MemoryPreference
            settings.MemorySetting = MemorySetting.MemoryPreference;

            // إنشاء ورقة عمل وإضافة بعض البيانات
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            worksheet.Cells["A2"].PutValue(123);

            // احفظ المصنف
            workbook.Save("MemorySettingExample.xlsx");

            Console.WriteLine("Workbook saved with MemorySetting.MemoryPreference.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


