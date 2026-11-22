---
title: "HtmlSaveOptions.MergeEmptyTdType"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. الخيار لدمج خلايا td الفارغة المتتالية. القيمة الافتراضية هي MergeEmptyTdType.Default"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/mergeemptytdtype/
---
## HtmlSaveOptions.MergeEmptyTdType property

الخيار لدمج الخلايا الفارغة المتجاورة (عناصر td الفارغة). القيمة الافتراضية هي MergeEmptyTdType.Default.

```csharp
public MergeEmptyTdType MergeEmptyTdType { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyMergeEmptyTdTypeDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // تعيين بيانات عينة
            worksheet.Cells["A1"].PutValue("Header1");
            worksheet.Cells["B1"].PutValue("Header2");
            worksheet.Cells["A2"].PutValue("Data1");
            worksheet.Cells["B2"].PutValue(""); // Empty cell

            // تكوين خيارات حفظ HTML باستخدام MergeEmptyTdType
            HtmlSaveOptions htmlOptions = new HtmlSaveOptions()
            {
                MergeEmptyTdType = MergeEmptyTdType.None // Demonstrate the property
            };

            // حفظ إلى HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, htmlOptions);

            Console.WriteLine("HTML saved with MergeEmptyTdType.None. Output file: " + outputPath);
        }
    }
}
```

### انظر أيضًا

* enum [MergeEmptyTdType](../../mergeemptytdtype/)
* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


