---
title: "تعداد OoxmlCompliance"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "تعداد Aspose.Cells.OoxmlCompliance. يسمح بتحديد أي مواصفة OOXML سيتم استخدامها عند الحفظ بصيغة Xlsx."
type: docs
url: /ar/net/aspose.cells/ooxmlcompliance/
---
## OoxmlCompliance enumeration

يسمح بتحديد أي مواصفة OOXML سيتم استخدامها عند الحفظ بتنسيق Xlsx.

```csharp
public enum OoxmlCompliance
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Ecma376_2006 | `0` | ECMA-376 الطبعة الأولى، 2006. |
| Iso29500_2008_Strict | `1` | مستوى التوافق الصارم ISO/IEC 29500:2008. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class OoxmlComplianceDemo
    {
        public static void OoxmlComplianceExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // الوصول إلى إعدادات المصنف
            WorkbookSettings settings = workbook.Settings;

            // حدد مستوى توافق OOXML إلى ISO/IEC 29500:2008 الصارم
            settings.Compliance = OoxmlCompliance.Iso29500_2008_Strict;

            // إضافة بعض البيانات إلى ورقة العمل
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells[0, 0].PutValue("Hello, World!");

            // احفظ المصنف بالمستوى المحدد لتوافق OOXML
            workbook.Save("OoxmlComplianceExample.xlsx");

            return;
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


