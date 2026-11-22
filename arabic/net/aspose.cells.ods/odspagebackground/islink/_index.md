---
title: "OdsPageBackground.IsLink"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsPageBackground. تشير إلى ما إذا كان رسمًا مرتبطًا"
type: docs
url: /ar/net/aspose.cells.ods/odspagebackground/islink/
---
## OdsPageBackground.IsLink property

يشير إلى ما إذا كانت رسمة مرتبطة.

```csharp
public bool IsLink { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Ods;
    using System;

    public class OdsPageBackgroundPropertyIsLinkDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook(FileFormatType.Ods);
            Worksheet worksheet = workbook.Worksheets[0];

            // الوصول إلى OdsPageBackground
            OdsPageBackground background = worksheet.PageSetup.ODSPageBackground;

            // عرض قيمة IsLink الحالية
            Console.WriteLine("Current IsLink value: " + background.IsLink);

            // تعديل خصائص الخلفية الحالية بدلاً من إنشاء واحدة جديدة
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicType = OdsPageBackgroundGraphicType.Position;
            background.GraphicPositionType = OdsPageBackgroundGraphicPositionType.TopLeft;
            background.LinkedGraphic = "path/to/image.png";

            // عرض قيمة IsLink الجديدة
            Console.WriteLine("New IsLink value: " + worksheet.PageSetup.ODSPageBackground.IsLink);

            // حفظ النتيجة
            workbook.Save("OdsPageBackgroundIsLinkDemo.ods");
        }
    }
}
```

### انظر أيضًا

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


