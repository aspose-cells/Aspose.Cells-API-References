---
title: "HtmlSaveOptions.CellCssPrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تحصل وتعيّن بادئة اسم CSS. القيمة الافتراضية هي"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/cellcssprefix/
---
## HtmlSaveOptions.CellCssPrefix property

يحصل على ويضبط بادئة اسم css، القيمة الافتراضية هي "".

```csharp
public string CellCssPrefix { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyCellCssPrefixDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // أضف بيانات تجريبية إلى الخلايا
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Age");
            worksheet.Cells["A2"].PutValue("John");
            worksheet.Cells["B2"].PutValue(30);

            // اضبط خيارات حفظ HTML مع CellCssPrefix
            HtmlSaveOptions saveOptions = new HtmlSaveOptions();
            saveOptions.CellCssPrefix = "custom-cell-";

            // حفظ دفتر العمل مع خيارات HTML
            workbook.Save("output.html", saveOptions);

            Console.WriteLine("HTML file saved with custom cell CSS prefix.");
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


