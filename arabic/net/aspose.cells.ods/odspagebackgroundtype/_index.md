---
title: "Enum OdsPageBackgroundType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundType enum. يمثل نوع خلفية الصفحة في ods"
type: docs
url: /ar/net/aspose.cells.ods/odspagebackgroundtype/
---
## OdsPageBackgroundType enumeration

يمثل نوع خلفية الصفحة في ملفات ods.

```csharp
public enum OdsPageBackgroundType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| None | `0` | بدون خلفية. |
| Color | `1` | يقوم بتنسيق الخلفية باللون. |
| Graphic | `2` | يقوم بتنسيق الخلفية بالصورة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundTypeDemo
    {
        public static void OdsPageBackgroundTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup للورقة
            PageSetup pageSetup = worksheet.PageSetup;

            // الوصول إلى خاصية ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // تعيين نوع الخلفية إلى اللون
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // تعيين لون الخلفية
            odsPageBackground.Color = Color.LightBlue;

            // احفظ المصنف
            workbook.Save("OdsPageBackgroundTypeExample.ods");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


