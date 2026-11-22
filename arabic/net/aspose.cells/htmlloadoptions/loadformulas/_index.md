---
title: "HtmlLoadOptions.LoadFormulas"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. تشير إلى ما إذا كان سيتم استيراد الصيغ إذا كان ملف HTML الأصلي يحتوي على صيغ"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/loadformulas/
---
## HtmlLoadOptions.LoadFormulas property

يشير إلى ما إذا كان يتم استيراد الصيغ إذا كان ملف HTML الأصلي يحتوي على صيغ

```csharp
public bool LoadFormulas { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyLoadFormulasDemo
    {
        public static void Run()
        {
            // أنشئ مثيلًا من HtmlLoadOptions
            HtmlLoadOptions loadOptions = new HtmlLoadOptions();

            // عيّن LoadFormulas إلى true لتحميل الصيغ من HTML
            loadOptions.LoadFormulas = true;

            // تحميل ملف HTML يحتوي على صيغ إلى مصنف
            Workbook workbook = new Workbook("input.html", loadOptions);

            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];

            // عرض الصيغة من الخلية A1 (إذا كانت موجودة في HTML)
            Console.WriteLine("Formula in A1: " + worksheet.Cells["A1"].Formula);

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


