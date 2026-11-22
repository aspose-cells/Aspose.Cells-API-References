---
title: "OoxmlSaveOptions.UpdateZoom"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية OoxmlSaveOptions. تشير إلى ما إذا كان يجب تحديث عامل التكبير قبل حفظ الملف إذا كانت خصائص PageSetup.FitToPagesWide و PageSetup.FitToPagesTall تتحكم في كيفية تكبير ورقة العمل"
type: docs
url: /ar/net/aspose.cells/ooxmlsaveoptions/updatezoom/
---
## OoxmlSaveOptions.UpdateZoom property

يشير إلى ما إذا كان يتم تحديث عامل التحجيم قبل حفظ الملف إذا كانت خصائص PageSetup.FitToPagesWide و PageSetup.FitToPagesTall تتحكم في كيفية تحجيم ورقة العمل.

```csharp
public bool UpdateZoom { get; set; }
```

### ملاحظات

القيمة الافتراضية هي false للأداء.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class OoxmlSaveOptionsPropertyUpdateZoomDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين مستوى التكبير الأولي
            worksheet.PageSetup.Zoom = 100;

            // إنشاء خيارات حفظ مع تمكين UpdateZoom
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx);
            saveOptions.UpdateZoom = true;

            // حفظ إلى تدفق الذاكرة
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, saveOptions);
                
                // إعادة تحميل المصنف للتحقق من تحديث التكبير
                stream.Position = 0;
                Workbook reloadedWorkbook = new Workbook(stream);
                Console.WriteLine("Worksheet zoom level: " + reloadedWorkbook.Worksheets[0].PageSetup.Zoom);
            }
        }
    }
}
```

### انظر أيضًا

* class [OoxmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


