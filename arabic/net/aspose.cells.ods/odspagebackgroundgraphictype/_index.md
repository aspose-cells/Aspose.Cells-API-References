---
title: "Enum OdsPageBackgroundGraphicType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.Ods.OdsPageBackgroundGraphicType enum. يمثل نوع تنسيق خلفية الصفحة باستخدام صورة"
type: docs
url: /ar/net/aspose.cells.ods/odspagebackgroundgraphictype/
---
## OdsPageBackgroundGraphicType enumeration

يمثل نوع تنسيق خلفية الصفحة مع صورة.

```csharp
public enum OdsPageBackgroundGraphicType
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| Position | `0` | تعيين الصورة في موقع محدد. |
| Area | `1` | تمديد الصورة. |
| Tile | `2` | كرر الصورة وكررها. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;
    using System.Drawing;

    public class OdsPageBackgroundGraphicTypeDemo
    {
        public static void OdsPageBackgroundGraphicTypeExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();

            // إضافة ورقة عمل جديدة إلى المصنف
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى PageSetup للورقة
            PageSetup pageSetup = worksheet.PageSetup;

            // الوصول إلى ODSPageBackground في PageSetup
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // تعيين لون الخلفية
            odsPageBackground.Color = Color.LightBlue;

            // تعيين نوع الرسم الخلفي إلى مبلط
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // تعيين مسار الرسم المرتبط (مع افتراض أن الصورة في نفس الدليل مع الملف التنفيذي)
            odsPageBackground.LinkedGraphic = "background_image.png";

            // احفظ المصنف
            workbook.Save("OdsPageBackgroundGraphicTypeExample.ods");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


