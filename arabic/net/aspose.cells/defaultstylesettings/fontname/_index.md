---
title: "DefaultStyleSettings.FontName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية DefaultStyleSettings. تحصل/تعين اسم الخط الافتراضي لدفتر العمل"
type: docs
url: /ar/net/aspose.cells/defaultstylesettings/fontname/
---
## DefaultStyleSettings.FontName property

الحصول/تعيين اسم الخط الافتراضي لدفتر العمل

```csharp
public string FontName { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class DefaultStyleSettingsPropertyFontNameDemo
    {
        public static void Run()
        {
            // إنشاء خيارات التحميل وتعيين اسم الخط
            LoadOptions loadOptions = new LoadOptions(LoadFormat.Xlsx);
            loadOptions.DefaultStyleSettings.FontName = "SimSun";

            // إنشاء دفتر عمل جديد باستخدام خيارات التحميل
            Workbook workbook = new Workbook();
            workbook.DefaultStyle.Font.Name = loadOptions.DefaultStyleSettings.FontName;

            // الوصول إلى النمط الافتراضي والتحقق من اسم الخط
            Style defaultStyle = workbook.DefaultStyle;
            Console.WriteLine("Default Font Name: " + defaultStyle.Font.Name);

            // إنشاء ورقة عمل وتعيين قيمة الخلية
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Font Name Test");

            // احفظ المصنف
            using (MemoryStream stream = new MemoryStream())
            {
                workbook.Save(stream, SaveFormat.Xlsx);
                Console.WriteLine("Workbook saved with default font: SimSun");
            }
        }
    }
}
```

### انظر أيضًا

* class [DefaultStyleSettings](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


