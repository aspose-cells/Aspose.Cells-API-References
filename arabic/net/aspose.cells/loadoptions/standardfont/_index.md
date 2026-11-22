---
title: "LoadOptions.StandardFont"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تعين اسم الخط القياسي الافتراضي"
type: docs
url: /ar/net/aspose.cells/loadoptions/standardfont/
---
## LoadOptions.StandardFont property

يعين اسم الخط القياسي الافتراضي

```csharp
[Obsolete("Use DefaultStyleSettings.FontName property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public string StandardFont { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام DefaultStyleSettings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2022. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontDemo
    {
        public static void Run()
        {
            // إنشاء ملف Excel تجريبي في الذاكرة
            MemoryStream ms = new MemoryStream();
            using (Workbook workbook = new Workbook())
            {
                workbook.Worksheets[0].Cells["A1"].PutValue("Standard Font Test");
                workbook.Save(ms, SaveFormat.Xlsx);
            }
            ms.Position = 0;

            // تعيين خيارات التحميل مع StandardFont
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.StandardFont = "SimSun";
            
            // تحميل دفتر العمل بالخط المحدد
            Workbook workbookWithFont = new Workbook(ms, loadOptions);
            
            // إظهار أن الخط تم تعيينه عن طريق فحص النمط الافتراضي
            Console.WriteLine("Default font after loading: " + 
                workbookWithFont.DefaultStyle.Font.Name);
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


