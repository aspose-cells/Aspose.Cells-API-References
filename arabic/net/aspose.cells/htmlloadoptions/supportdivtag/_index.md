---
title: "HtmlLoadOptions.SupportDivTag"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. تشير إلى ما إذا كان يدعم تخطيط علامة div عندما يحتوي ملف HTML عليها. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/supportdivtag/
---
## HtmlLoadOptions.SupportDivTag property

يشير إلى ما إذا كان يدعم تخطيط الوسم `<div>` عندما يحتوي ملف HTML عليه. القيمة الافتراضية هي false.

```csharp
public bool SupportDivTag { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertySupportDivTagDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML مع تمكين SupportDivTag
            HtmlLoadOptions htmlLoadOptions = new HtmlLoadOptions(LoadFormat.Html);
            htmlLoadOptions.SupportDivTag = true;

            // تحميل ملف HTML مع علامات div
            Workbook workbook = new Workbook("input.html", htmlLoadOptions);

            // الوصول إلى البيانات من ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cell cell = worksheet.Cells["A1"];
            
            // إخراج قيمة الخلية ومعلومات النمط
            Console.WriteLine("Cell A1 value: " + cell.StringValue);
            Console.WriteLine("Is bold: " + cell.GetStyle().Font.IsBold);

            // حفظ كملف Excel
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


