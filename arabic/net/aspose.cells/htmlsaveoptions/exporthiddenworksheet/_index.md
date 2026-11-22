---
title: "HtmlSaveOptions.ExportHiddenWorksheet"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية HtmlSaveOptions. تشير إلى تصدير محتوى ورقة العمل المخفية. القيمة الافتراضية هي true"
type: docs
url: /ar/net/aspose.cells/htmlsaveoptions/exporthiddenworksheet/
---
## HtmlSaveOptions.ExportHiddenWorksheet property

تشير إلى ما إذا كان يتم تصدير محتوى ورقة العمل المخفي. القيمة الافتراضية هي true.

```csharp
public bool ExportHiddenWorksheet { get; set; }
```

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class HtmlSaveOptionsPropertyExportHiddenWorksheetDemo
    {
        public static void Run()
        {
            // أنشئ مصنفًا ببيانات تجريبية
            Workbook workbook = new Workbook();
            Worksheet worksheet1 = workbook.Worksheets[0];
            worksheet1.Name = "VisibleSheet";
            worksheet1.Cells["A1"].PutValue("Visible Data");

            Worksheet worksheet2 = workbook.Worksheets.Add("HiddenSheet");
            worksheet2.Cells["A1"].PutValue("Hidden Data");
            worksheet2.IsVisible = false;

            // حدد خيارات حفظ HTML
            HtmlSaveOptions saveOptions = new HtmlSaveOptions
            {
                ExportHiddenWorksheet = false, // Don't export hidden worksheets
                ExportActiveWorksheetOnly = false
            };

            // احفظ مع عدم تصدير ورقة العمل المخفية
            workbook.Save("output_without_hidden.html", saveOptions);

            // غيّر الخيار لتصدير أوراق العمل المخفية
            saveOptions.ExportHiddenWorksheet = true;

            // احفظ مع تصدير ورقة العمل المخفية
            workbook.Save("output_with_hidden.html", saveOptions);
        }
    }
}
```

### انظر أيضًا

* class [HtmlSaveOptions](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


