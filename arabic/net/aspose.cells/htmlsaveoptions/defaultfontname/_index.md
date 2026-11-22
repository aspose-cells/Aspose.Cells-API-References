---
title: "HtmlSaveOptions.DefaultFontName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. حدد اسم الخط الافتراضي لتصدير html. سيُستخدم الخط الافتراضي عندما لا يكون خط النمط موجودًا. إذا كانت هذه الخاصية null سيستخدم Aspose.Cells خطًا عالميًا له نفس عائلة الخط الأصلي. القيمة الافتراضية هي null"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/defaultfontname/
---
## HtmlSaveOptions.DefaultFontName property

حدد اسم الخط الافتراضي لتصدير html، سيُستخدم الخط الافتراضي عندما لا يكون خط النمط موجودًا، إذا كانت هذه الخاصية null، سيستخدم Aspose.Cells خطًا عالميًا يملك نفس عائلة الخط الأصلي، القيمة الافتراضية هي null.

```csharp
public string DefaultFontName { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyDefaultFontNameDemo
    {
        public static void Run()
        {
            // إنشاء مصنف تجريبي
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية
            worksheet.Cells["A1"].PutValue("Sample Text");
            
            // ضبط خيارات حفظ HTML بخط افتراضي مخصص
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.DefaultFontName = "Courier New";
            
            // حفظ إلى HTML بالخط المحدد
            workbook.Save("output.html", saveOptions);
            
            Console.WriteLine("HTML file saved with default font: " + saveOptions.DefaultFontName);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


