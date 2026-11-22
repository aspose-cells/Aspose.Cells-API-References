---
title: "HtmlSaveOptions.ExportFormula"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى ما إذا كان سيتم تصدير الصيغة عند حفظ الملف إلى html. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html الناتج إلى Excel يرجى الحفاظ على القيمة الافتراضية"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exportformula/
---
## HtmlSaveOptions.ExportFormula property

تشير إلى ما إذا كان يتم تصدير الصيغ عند حفظ الملف إلى html. القيمة الافتراضية هي true. إذا كنت تريد استيراد ملف html الناتج إلى Excel، يرجى الحفاظ على القيمة الافتراضية.

```csharp
public bool ExportFormula { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportFormulaDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // أضف بيانات تجريبية وصيغة
            worksheet.Cells["A1"].PutValue("Value 1");
            worksheet.Cells["B1"].PutValue("Value 2");
            worksheet.Cells["C1"].Formula = "=A1+B1";
            worksheet.Cells["A2"].PutValue(10);
            worksheet.Cells["B2"].PutValue(20);
            worksheet.Cells["C2"].Formula = "=A2+B2";

            // احفظ مع ExportFormula = true
            HtmlSaveOptions options1 = new HtmlSaveOptions();
            options1.ExportFormula = true;
            workbook.Save("output_with_formulas.html", options1);

            // احفظ مع ExportFormula = false
            HtmlSaveOptions options2 = new HtmlSaveOptions();
            options2.ExportFormula = false;
            workbook.Save("output_without_formulas.html", options2);

            // تحقق من النتائج
            string htmlWithFormulas = File.ReadAllText("output_with_formulas.html");
            string htmlWithoutFormulas = File.ReadAllText("output_without_formulas.html");

            Console.WriteLine("HTML with formulas contains formula: " + 
                htmlWithFormulas.Contains("=A2+B2"));
            Console.WriteLine("HTML without formulas contains formula: " + 
                htmlWithoutFormulas.Contains("=A2+B2"));
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


