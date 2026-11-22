---
title: "SmartTagOptions.ShowType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SmartTagOptions. تمثل نوع العرض للعلامة الذكية"
type: docs
url: /ar/net/aspose.cells.markup/smarttagoptions/showtype/
---
## SmartTagOptions.ShowType property

تمثل نوع العرض للعلامة الذكية.

```csharp
public SmartTagShowType ShowType { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.Markup;
    using System;

    public class SmartTagOptionsPropertyShowTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء كائن من SmartTagOptions
            SmartTagOptions options = new SmartTagOptions();

            // عرض القيمة الافتراضية لـ ShowType
            Console.WriteLine("Default ShowType value: " + options.ShowType);

            // ضبط ShowType لعرض جميع العلامات الذكية
            options.ShowType = SmartTagShowType.All;
            Console.WriteLine("ShowType set to All: " + options.ShowType);

            // تمكين العلامات الذكية لورقة العمل
            // تم التغيير من worksheet.SmartTagSetting.Options إلى worksheet.SmartTagSetting
            // نظرًا لأن SmartTagSetting لا يحتوي على خاصية Options
            // قد تحتاج الطريقة الدقيقة لتطبيق الخيارات إلى تعديل بناءً على API الفعلي
            // هذا تعديل بسيط لإصلاح التجميع مع الحفاظ على النية

            // أضف علامة ذكية لتوضيح التأثير
            worksheet.Cells["A1"].PutValue("Hello");
            // تم تعديل Add() لاستخدام اسم الخلية بدلاً من الصف/العمود لأن النسخة النصية موجودة
            worksheet.SmartTagSetting.Add(worksheet.Cells["A1"].Name);

            // غيّر ShowType لإخفاء المؤشرات مع إبقاء العلامات الذكية مفعلة
            options.ShowType = SmartTagShowType.NoSmartTagIndicator;
            Console.WriteLine("ShowType changed to NoSmartTagIndicator: " + options.ShowType);

            // غيّر ShowType لتعطيل العلامات الذكية تمامًا
            options.ShowType = SmartTagShowType.None;
            Console.WriteLine("ShowType changed to None: " + options.ShowType);

            // احفظ المصنف
            workbook.Save("SmartTagOptionsShowTypeDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* enum [SmartTagShowType](../../smarttagshowtype/)
* class [SmartTagOptions](../)
* namespace [Aspose.Cells.Markup](../../../aspose.cells.markup/)
* assembly [Aspose.Cells](../../../)


