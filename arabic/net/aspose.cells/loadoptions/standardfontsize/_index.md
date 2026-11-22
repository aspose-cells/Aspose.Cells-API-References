---
title: "LoadOptions.StandardFontSize"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LoadOptions. تُعيّن حجم الخط القياسي الافتراضي"
type: docs
url: /ar/net/aspose.cells/loadoptions/standardfontsize/
---
## LoadOptions.StandardFontSize property

يُعيّن حجم الخط القياسي الافتراضي.

```csharp
[Obsolete("Use DefaultStyleSettings.FontSize property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public double StandardFontSize { get; set; }
```

### ملاحظات

ملاحظة: هذا العضو الآن غير صالح. بدلاً من ذلك، يرجى استخدام DefaultStyleSettings. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2022. تُعرب Aspose عن أسفها لأي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class LoadOptionsPropertyStandardFontSizeDemo
    {
        public static void Run()
        {
            // أنشئ خيارات تحميل HTML واضبط StandardFontSize
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            loadOptions.StandardFont = "Calibri";
            loadOptions.StandardFontSize = 11;

            // حمّل دفتر العمل باستخدام الخيارات
            Workbook workbook = new Workbook(new MemoryStream(), loadOptions);
            
            // الوصول إلى ورقة العمل الأولى والخلايا
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // عيّن بعض النصوص التجريبية وتحقق من خصائص الخط
            cells["A1"].PutValue("Sample Text");
            Style style = cells["A1"].GetStyle();
            
            Console.WriteLine("Font Name: " + style.Font.Name);
            Console.WriteLine("Font Size: " + style.Font.Size);
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


