---
title: "HtmlLoadOptions.AutoFitColsAndRows"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. تشير إلى ما إذا كان سيتم ضبط الأعمدة والصفوف تلقائيًا. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/autofitcolsandrows/
---
## HtmlLoadOptions.AutoFitColsAndRows property

يشير إلى ما إذا كان سيتم ضبط الأعمدة والصفوف تلقائيًا. القيمة الافتراضية هي false.

```csharp
public bool AutoFitColsAndRows { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyAutoFitColsAndRowsDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // تمكين الضبط التلقائي للأعمدة والصفوف
            loadOptions.AutoFitColsAndRows = true;
            
            // تحميل ملف HTML باستخدام الخيارات المحددة
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            
            // سيتم تطبيق الضبط التلقائي للأعمدة والصفوف أثناء التحميل
            Console.WriteLine("Columns and rows have been auto-fitted during HTML import.");
            
            // احفظ المصنف
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


