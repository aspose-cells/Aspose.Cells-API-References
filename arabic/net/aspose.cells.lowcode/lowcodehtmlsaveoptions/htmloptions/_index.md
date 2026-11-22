---
title: "LowCodeHtmlSaveOptions.HtmlOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeHtmlSaveOptions. الخيارات العامة لحفظ html"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/
---
## LowCodeHtmlSaveOptions.HtmlOptions property

الخيارات العامة لحفظ HTML.

```csharp
public HtmlSaveOptions HtmlOptions { get; set; }
```

### ملاحظات

عند تحديد مثال واحد من [`HtmlSaveOptions`](../../../aspose.cells/htmlsaveoptions/)، سيتم استبدال [`SaveFormat`](../saveformat/) (إذا كان قد تم تحديده مسبقًا).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertyHtmlOptionsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Apple");
            worksheet.Cells["B2"].PutValue(2.99);
            
            // إنشاء خيارات حفظ HTML منخفضة الشيفرة
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                SaveFormat = SaveFormat.Html,
                HtmlOptions = new HtmlSaveOptions()
            };

            // عرض إعداد تصدير خطوط الشبكة الحالية
            Console.WriteLine("Export gridlines initially: " + saveOptions.HtmlOptions.ExportGridLines);

            // حفظ مع إظهار خطوط الشبكة
            workbook.Save("HtmlWithGridlines.html", saveOptions.HtmlOptions);

            // تعديل خيارات HTML لإخفاء خطوط الشبكة
            saveOptions.HtmlOptions = new HtmlSaveOptions { ExportGridLines = false };
            Console.WriteLine("Export gridlines after modification: " + saveOptions.HtmlOptions.ExportGridLines);

            // حفظ بدون خطوط الشبكة
            workbook.Save("HtmlWithoutGridlines.html", saveOptions.HtmlOptions);

            Console.WriteLine("Demo executed successfully. Compare output files.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../../../aspose.cells/htmlsaveoptions/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


