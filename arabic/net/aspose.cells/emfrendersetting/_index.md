---
title: "التعداد EmfRenderSetting"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "التعداد Aspose.Cells.EmfRenderSetting. إعداد لتصيير ملف Emf"
type: docs
url: /ar/net/aspose.cells/emfrendersetting/
---
## EmfRenderSetting enumeration

إعداد لتصوير ملف Emf الميتا.

```csharp
public enum EmfRenderSetting
```

### القيم

| الاسم | القيمة | الوصف |
| --- | --- | --- |
| EmfOnly | `0` | تصيير سجلات Emf فقط. |
| EmfPlusPrefer | `1` | يفضل تصيير سجلات EmfPlus. |

### أمثلة

```csharp
using System;
using Aspose.Cells;
using Aspose.Cells.Rendering;

namespace AsposeCellsExamples
{
    public class CellsClassEmfRenderSettingDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("EMF Render Setting Demo");
            worksheet.Cells["A2"].PutValue("Using EmfOnly setting");

            // إنشاء خيارات صورة باستخدام إعداد تصيير EMF
            ImageOrPrintOptions options = new ImageOrPrintOptions
            {
                EmfRenderSetting = EmfRenderSetting.EmfOnly
            };

            // إنشاء تصيير ورقة باستخدام الخيارات
            SheetRender render = new SheetRender(worksheet, options);

            // حفظ الصفحة الأولى كصورة EMF
            render.ToImage(0, "EmfRenderSettingDemo.emf");

            Console.WriteLine("EMF file created successfully with EmfOnly setting.");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


