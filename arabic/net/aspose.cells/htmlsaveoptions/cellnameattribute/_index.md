---
title: "HtmlSaveOptions.CellNameAttribute"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تحدد السمة التي تشير إلى اسم الخلية (CellName) الذي سيُكتب. مثال: إذا كانت القيمة id فإن الخلية A1 سيصبح الناتج td idA1. القيمة الافتراضية هي null"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/cellnameattribute/
---
## HtmlSaveOptions.CellNameAttribute property

يحدد السمة التي تشير إلى CellName التي سيتم كتابتها. (مثال: إذا كانت القيمة "id"، فبالنسبة للخلية "A1" سيكون الناتج:&lt;td id='A1'&gt;). القيمة الافتراضية هي null.

```csharp
public string CellNameAttribute { get; set; }
```

### أمثلة

```csharp
using System;
using System.IO;
using System.Text.RegularExpressions;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellNameAttributeDemo
    {
        public static void Run()
        {
            // أنشئ دفتر عمل تجريبي يحتوي على بعض البيانات
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Test Data");
            worksheet.Cells["B2"].PutValue(123);

            // اضبط خيارات حفظ HTML مع CellNameAttribute
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellNameAttribute = "id";
            saveOptions.ExportImagesAsBase64 = true;
            saveOptions.ExportActiveWorksheetOnly = true;

            // حفظ إلى ملف HTML
            string outputPath = "output.html";
            workbook.Save(outputPath, saveOptions);

            // تحقق من أن مخرجات HTML تحتوي على معرفات الخلايا
            string htmlContent = File.ReadAllText(outputPath);
            Console.WriteLine("HTML contains A1 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='A1'"));
            Console.WriteLine("HTML contains B2 cell with ID: " + Regex.IsMatch(htmlContent, @"<td\s+id='B2'"));
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


