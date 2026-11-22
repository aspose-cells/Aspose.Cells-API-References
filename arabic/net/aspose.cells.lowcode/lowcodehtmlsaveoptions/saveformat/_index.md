---
title: "LowCodeHtmlSaveOptions.SaveFormat"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeHtmlSaveOptions. تحصل وتعيّن تنسيق جدول البيانات"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/
---
## LowCodeHtmlSaveOptions.SaveFormat property

يحصل ويضبط تنسيق جدول البيانات.

```csharp
public override SaveFormat SaveFormat { get; set; }
```

### ملاحظات

عند تغيير هذه الخاصية، سيتم تجاهل تنسيق الحفظ المحدد بواسطة [`HtmlOptions`](../htmloptions/) (إذا كان قد تم تحديده مسبقًا).

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeHtmlSaveOptionsPropertySaveFormatDemo
    {
        public static void Run()
        {
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample HTML Export");

            LowCodeHtmlSaveOptions options = new LowCodeHtmlSaveOptions();
            Console.WriteLine("Current SaveFormat value: " + options.SaveFormat);

            options.SaveFormat = SaveFormat.Html;
            options.HtmlOptions = new HtmlSaveOptions();

            workbook.Save("LowCodeHtmlExport.html", options.HtmlOptions);
        }
    }
}
```

### انظر أيضًا

* enum [SaveFormat](../../../aspose.cells/saveformat/)
* class [LowCodeHtmlSaveOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


