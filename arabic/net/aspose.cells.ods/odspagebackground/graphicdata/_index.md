---
title: "OdsPageBackground.GraphicData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OdsPageBackground. تحصل وتعيّن بيانات الرسم"
type: docs
url: /ar/net/aspose.cells.ods/odspagebackground/graphicdata/
---
## OdsPageBackground.GraphicData property

يحصل ويضبط بيانات الرسومات.

```csharp
public byte[] GraphicData { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;
using Aspose.Cells.Ods;

namespace AsposeCellsExamples
{
    public class OdsPageBackgroundPropertyGraphicDataDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // الوصول إلى ورقة العمل الأولى وإعدادات صفحتها
            Worksheet worksheet = workbook.Worksheets[0];
            PageSetup pageSetup = worksheet.PageSetup;
            
            // تعيين خصائص خلفية صفحة ODS
            OdsPageBackground background = pageSetup.ODSPageBackground;
            background.Type = OdsPageBackgroundType.Graphic;
            
            // تحميل بيانات الصورة وتعيينها كخلفية
            string imagePath = "sample.png"; // Replace with actual image path
            if (File.Exists(imagePath))
            {
                background.GraphicData = File.ReadAllBytes(imagePath);
                background.GraphicType = OdsPageBackgroundGraphicType.Area;
                
                // احفظ المصنف
                workbook.Save("output.ods");
                
                Console.WriteLine("ODS file with graphic background created successfully.");
            }
            else
            {
                Console.WriteLine("Image file not found: " + imagePath);
            }
        }
    }
}
```

### انظر أيضًا

* class [OdsPageBackground](../)
* namespace [Aspose.Cells.Ods](../../../aspose.cells.ods/)
* assembly [Aspose.Cells](../../../)


