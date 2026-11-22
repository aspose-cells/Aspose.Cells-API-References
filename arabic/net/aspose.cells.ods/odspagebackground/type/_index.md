---
title: "OdsPageBackground.Type"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsPageBackground. تحصل وتضبط نوع خلفية الصفحة"
type: docs
url: /ar/net/aspose.cells.ods/odspagebackground/type/
---
## OdsPageBackground.Type property

يحصل ويضبط نوع خلفية الصفحة.

```csharp
public OdsPageBackgroundType Type { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى إعداد صفحة الورقة الأولى
            PageSetup ps = workbook.Worksheets[0].PageSetup;
            
            // احصل على خلفية صفحة ODS
            OdsPageBackground background = ps.ODSPageBackground;
            
            // ضبط نوع الخلفية إلى رسم وتكوينه
            background.Type = OdsPageBackgroundType.Graphic;
            background.GraphicData = File.ReadAllBytes("image1.png");
            background.GraphicType = OdsPageBackgroundGraphicType.Area;
            
            // احفظ المصنف
            workbook.Save("output.ods");
            
            // إعادة تحميل الملف المحفوظ للتحقق من الإعدادات
            Workbook verifyWorkbook = new Workbook("output.ods");
            PageSetup verifyPs = verifyWorkbook.Worksheets[0].PageSetup;
            OdsPageBackground verifyBackground = verifyPs.ODSPageBackground;
            
            // إخراج نتائج التحقق
            Console.WriteLine("Background Type: " + verifyBackground.Type);
            Console.WriteLine("Graphic Type: " + verifyBackground.GraphicType);
        }
    }
}
```

### انظر أيضًا

* enum [OdsPageBackgroundType](../../odspagebackgroundtype/)
* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


