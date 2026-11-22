---
title: "الفئة SmartTagSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Markup.SmartTagSetting. تمثل جميع كائنات SmartTagCollection في ورقة العمل"
type: docs
url: /ar/net/aspose.cells.markup/smarttagsetting/
---
## SmartTagSetting class

تمثل جميع كائنات [`SmartTagCollection`](../smarttagcollection/) في ورقة العمل.

```csharp
public class SmartTagSetting : CollectionBase
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Item](../../aspose.cells.markup/smarttagsetting/item/) { get; } | يحصل على كائن [`SmartTagCollection`](../smarttagcollection/) حسب الفهرس. (3 فهارس) |

## الطرق

| الاسم | الوصف |
| --- | --- |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add_1)(string) | إضافة علامة ذكية للخلية. |
| [Add](../../aspose.cells.markup/smarttagsetting/add/#add)(int, int) | يضيف كائن [`SmartTagCollection`](../smarttagcollection/) إلى خلية. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagSettingDemo
    {
        public static void SmartTagSettingExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة علامة ذكية إلى خلية محددة
            SmartTagSetting smartTagSetting = worksheet.SmartTagSetting;
            int smartTagIndex = smartTagSetting.Add(0, 0); // Adding smart tag to cell A1

            // الوصول إلى SmartTagCollection للخلية
            SmartTagCollection smartTagCollection = smartTagSetting[0, 0];

            // إضافة علامة ذكية إلى المجموعة
            int tagIndex = smartTagCollection.Add("urn:schemas-microsoft-com:office:smarttags", "date");

            // تعيين سعة إعداد العلامة الذكية
            smartTagSetting.Capacity = 10;

            // طباعة عدد العلامات الذكية
            Console.WriteLine("Total Smart Tags: " + smartTagSetting.Count);

            // احفظ المصنف
            workbook.Save("SmartTagSettingExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Markup](../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../)


