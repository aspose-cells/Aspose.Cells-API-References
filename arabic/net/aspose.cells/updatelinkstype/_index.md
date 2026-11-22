---
title: "التعداد UpdateLinksType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.UpdateLinksType. يمثل طريقة تحديث الروابط إلى دفاتر عمل أخرى عند فتح دفتر العمل"
type: docs
url: /ar/net/aspose.cells/updatelinkstype/
---
## UpdateLinksType enumeration

يمثل طريقة تحديث الروابط إلى مصنفات أخرى عند فتح المصنف.

```csharp
public enum UpdateLinksType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| UserSet | `0` | مطالبة المستخدم بالتحديث. |
| Never | `1` | عدم التحديث، وعدم مطالبة المستخدم. |
| Always | `2` | تحديث دائمًا. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class UpdateLinksTypeDemo
    {
        public static void UpdateLinksTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات دفتر العمل
            WorkbookSettings settings = workbook.Settings;

            // تعيين UpdateLinksType إلى تحديث دائمًا
            settings.UpdateLinksType = UpdateLinksType.Always;

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // إضافة بيانات عينة إلى ورقة العمل
            worksheet.Cells["A1"].PutValue("External Link Example");
            worksheet.Cells["A2"].PutValue("Data");

            // احفظ المصنف
            workbook.Save("UpdateLinksTypeExample.xlsx");

            // إخراج إعداد UpdateLinksType الحالي
            Console.WriteLine("UpdateLinksType is set to: " + settings.UpdateLinksType);
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


