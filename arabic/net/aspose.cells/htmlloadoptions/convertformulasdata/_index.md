---
title: "HtmlLoadOptions.ConvertFormulasData"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. إذا كانت true يتم تحويل السلسلة إلى صيغة عندما يبدأ قيمة السلسلة بحرف. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/convertformulasdata/
---
## HtmlLoadOptions.ConvertFormulasData property

إذا كانت true، يتم تحويل السلسلة إلى صيغة عندما يبدأ قيمة السلسلة بالحرف '=', والقيمة الافتراضية هي false.

```csharp
[Obsolete("Use HtmlLoadOptions.HasFormula property instead.")]
[EditorBrowsable(EditorBrowsableState.Never)]
public bool ConvertFormulasData { get; set; }
```

### ملاحظات

ملاحظة: هذه الخاصية أصبحت الآن غير صالحة. بدلاً من ذلك، يرجى استخدام خاصية HtmlLoadOptions.HasFormula. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ مارس 2023. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyConvertFormulasDataDemo
    {
        public static void Run()
        {
            // أنشئ مثيلًا من HtmlLoadOptions
            HtmlLoadOptions options = new HtmlLoadOptions();

            // عيّن خاصية ConvertFormulasData إلى true
            options.ConvertFormulasData = true;

            // تحميل ملف HTML إلى مصنف باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("input.html", options);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض بعض قيم الخلايا لتوضيح تحويل الصيغ
            Console.WriteLine("Cell A1 value: " + worksheet.Cells["A1"].Value);
            Console.WriteLine("Cell B1 formula: " + worksheet.Cells["B1"].Formula);

            // حفظ المصنف إلى ملف Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


