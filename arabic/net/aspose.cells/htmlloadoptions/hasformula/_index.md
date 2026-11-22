---
title: "HtmlLoadOptions.HasFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlLoadOptions. تشير إلى ما إذا كان النص صيغة إذا بدأ بـ"
type: docs
url: /ar/net/aspose.cells/htmlloadoptions/hasformula/
---
## HtmlLoadOptions.HasFormula property

يشير إلى ما إذا كان النص صيغة إذا بدأ بـ "=".

```csharp
public bool HasFormula { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlLoadOptionsPropertyHasFormulaDemo
    {
        public static void Run()
        {
            // إنشاء خيارات تحميل HTML
            HtmlLoadOptions loadOptions = new HtmlLoadOptions(LoadFormat.Html);
            
            // عيّن HasFormula إلى false لمعالجة سلاسل الصيغ كنص عادي
            loadOptions.HasFormula = false;
            
            // إنشاء مصنف باستخدام ملف HTML وخيارات التحميل
            Workbook workbook = new Workbook("example.html", loadOptions);
            
            // الوصول إلى ورقة العمل الأولى
            Worksheet worksheet = workbook.Worksheets[0];
            Cells cells = worksheet.Cells;
            
            // عرض بعض قيم الخلايا لتوضيح استيراد HTML
            Console.WriteLine("A1: " + cells["A1"].StringValue);
            Console.WriteLine("B1: " + cells["B1"].StringValue);
            
            // حفظ كـ XLSX
            workbook.Save("output.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [HtmlLoadOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


