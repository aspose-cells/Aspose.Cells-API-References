---
title: "HtmlSaveOptions.HtmlCrossStringType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم عرض سلسلة عبر الخلايا بنفس طريقة MS Excel عند حفظ ملف Excel بتنسيق html. بشكل افتراضي القيمة هي Default لذا بالنسبة لسلاسل عبر الخلايا هناك فرق بسيط بين ملفات html التي تنشئها Aspose.Cells و MS Excel. ولكن الأداء لإنشاء ملفات html كبيرة عند ضبط القيمة إلى Cross سيكون أسرع عدة مرات مقارنةً بضبطها إلى Default أو Fit2Cell"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/htmlcrossstringtype/
---
## HtmlSaveOptions.HtmlCrossStringType property

يشير إلى ما إذا كان سيتم عرض سلسلة عبر الخلايا بنفس طريقة MS Excel عند حفظ ملف Excel بصيغة html. بشكل افتراضي القيمة هي Default، لذا بالنسبة لسلاسل عبر الخلايا، هناك فرق بسيط بين ملفات html التي تم إنشاؤها بواسطة Aspose.Cells و MS Excel. لكن الأداء لإنشاء ملفات html الكبيرة، ضبط القيمة إلى Cross سيكون أسرع عدة مرات مقارنةً بضبطها إلى Default أو Fit2Cell.

```csharp
public HtmlCrossType HtmlCrossStringType { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyHtmlCrossStringTypeDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // إضافة بيانات نموذجية ستظهر سلوك السلسلة عبر الخلايا
            worksheet.Cells["A1"].PutValue("Left Content");
            worksheet.Cells["B1"].PutValue("Right Content");
            
            // الحصول على أنماط الخلايا وتعديلها
            Style styleA1 = worksheet.Cells["A1"].GetStyle();
            styleA1.Borders[BorderType.RightBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["A1"].SetStyle(styleA1);
            
            Style styleB1 = worksheet.Cells["B1"].GetStyle();
            styleB1.Borders[BorderType.LeftBorder].LineStyle = CellBorderType.Thin;
            worksheet.Cells["B1"].SetStyle(styleB1);

            // تكوين خيارات حفظ HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.HtmlCrossStringType = HtmlCrossType.CrossHideRight;

            // حفظ المصنف إلى HTML
            workbook.Save("output.html", options);
            
            Console.WriteLine("HTML file saved with CrossHideRight option.");
        }
    }
}
```

### انظر أيضًا

* enum [HtmlCrossType](../../htmlcrosstype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


