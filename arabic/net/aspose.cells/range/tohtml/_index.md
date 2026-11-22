---
title: "Range.ToHtml"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة Range. تحويل النطاق إلى html"
type: docs
url: /ar/net/aspose.cells/range/tohtml/
---
## Range.ToHtml method

تحويل النطاق إلى html.

```csharp
public byte[] ToHtml(HtmlSaveOptions saveOptions)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| saveOptions | HtmlSaveOptions | خيارات تحويل النطاق إلى html. |

### أمثلة

```csharp
using System;
using System.IO;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class RangeMethodToHtmlWithHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء بعض البيانات في النطاق A1:J25
            for (int i = 0; i < 25; i++)
            {
                for (int j = 0; j < 10; j++)
                {
                    worksheet.Cells[i, j].Value = $"Cell {i+1},{j+1}";
                }
            }

            // إنشاء نطاق باسم نوع مؤهل بالكامل
            Aspose.Cells.Range range = worksheet.Cells.CreateRange("A1:J25");
            
            // إنشاء خيارات حفظ HTML
            HtmlSaveOptions options = new HtmlSaveOptions();
            options.ExportImagesAsBase64 = true;
            
            // تحويل النطاق إلى HTML
            byte[] htmlData = range.ToHtml(options);
            
            // حفظ HTML إلى ملف
            File.WriteAllBytes("output.html", htmlData);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../../htmlsaveoptions/)
* class [Range](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


