---
title: "الفئة OdsPageBackground"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.Ods.OdsPageBackground. تمثل خلفية الصفحة في ods"
type: docs
url: /ar/net/aspose.cells.ods/odspagebackground/
---
## OdsPageBackground class

يمثل خلفية الصفحة في ods.

```csharp
public class OdsPageBackground
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [OdsPageBackground](odspagebackground/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [Color](../../aspose.cells.ods/odspagebackground/color/) { get; set; } | يحصل ويضبط لون الخلفية. |
| [GraphicData](../../aspose.cells.ods/odspagebackground/graphicdata/) { get; set; } | يحصل ويضبط بيانات الرسومات. |
| [GraphicPositionType](../../aspose.cells.ods/odspagebackground/graphicpositiontype/) { get; set; } | يحصل ويضبط موضع الرسمة الخلفية. |
| [GraphicType](../../aspose.cells.ods/odspagebackground/graphictype/) { get; set; } | يحصل ويضبط نوع رسمة خلفية الصفحة. |
| [IsLink](../../aspose.cells.ods/odspagebackground/islink/) { get; } | يشير إلى ما إذا كانت رسمة مرتبطة. |
| [LinkedGraphic](../../aspose.cells.ods/odspagebackground/linkedgraphic/) { get; set; } | يحصل ويضبط مسار الرسمة المرتبطة. |
| [Type](../../aspose.cells.ods/odspagebackground/type/) { get; set; } | يحصل ويضبط نوع خلفية الصفحة. |

### أمثلة

```csharp
using Aspose.Cells;
using Aspose.Cells.Ods;
using System;
using System.Drawing;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundDemo
    {
        public static void OdsPageBackgroundExample()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // الوصول إلى كائن PageSetup
            PageSetup pageSetup = sheet.PageSetup;

            // الوصول إلى كائن ODSPageBackground
            OdsPageBackground odsPageBackground = pageSetup.ODSPageBackground;

            // تعيين نوع الخلفية إلى اللون
            odsPageBackground.Type = OdsPageBackgroundType.Color;

            // تعيين لون الخلفية
            odsPageBackground.Color = Color.LightBlue;

            // تعيين نوع رسمة الخلفية
            odsPageBackground.GraphicType = OdsPageBackgroundGraphicType.Tile;

            // تعيين موضع رسمة الخلفية
            odsPageBackground.GraphicPositionType = OdsPageBackgroundGraphicPositionType.CenterCenter;

            // تعيين مسار الرسمة المرتبطة (إن وجد)
            odsPageBackground.LinkedGraphic = "path/to/graphic.png";

            // احفظ المصنف
            workbook.Save("OdsPageBackgroundExample.ods");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.Ods](../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../)


