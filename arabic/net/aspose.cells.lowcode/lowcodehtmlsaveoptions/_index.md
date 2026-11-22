---
title: "الفئة LowCodeHtmlSaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.LowCode.LowCodeHtmlSaveOptions. خيارات لحفظ HTML بطريقة منخفضة الكود"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodehtmlsaveoptions/
---
## LowCodeHtmlSaveOptions class

خيارات حفظ html بطريقة منخفضة الكود.

```csharp
public class LowCodeHtmlSaveOptions : LowCodeSaveOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodeHtmlSaveOptions](lowcodehtmlsaveoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [HtmlOptions](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/htmloptions/) { get; set; } | الخيارات العامة لحفظ HTML. |
| [OutputFile](../../aspose.cells.lowcode/lowcodesaveoptions/outputfile/) { get; set; } | الحصول وتعيين الملف (مع المسار إذا لزم) لحفظ البيانات المُولدة. عند تعيين هذه الخاصية بقيمة غير null أو سلسلة فارغة، سيتم تجاهل [`OutputStream`](../lowcodesaveoptions/outputstream/). (موروث من [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| [OutputStream](../../aspose.cells.lowcode/lowcodesaveoptions/outputstream/) { get; set; } | الحصول وتعيين الدفق لكتابة البيانات المُولدة إليه. عند تعيين هذه الخاصية بقيمة غير null، سيتم تجاهل [`OutputFile`](../lowcodesaveoptions/outputfile/). (موروث من [`LowCodeSaveOptions`](../lowcodesaveoptions/).) |
| override [SaveFormat](../../aspose.cells.lowcode/lowcodehtmlsaveoptions/saveformat/) { get; set; } | يحصل ويضبط تنسيق جدول البيانات. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeHtmlSaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Product");
            worksheet.Cells["B1"].PutValue("Price");
            worksheet.Cells["A2"].PutValue("Widget");
            worksheet.Cells["B2"].PutValue(29.99);

            // إنشاء وتكوين LowCodeHtmlSaveOptions
            LowCodeHtmlSaveOptions saveOptions = new LowCodeHtmlSaveOptions
            {
                HtmlOptions = new HtmlSaveOptions()
                {
                    ExportWorksheetCSSSeparately = false,
                    ExportImagesAsBase64 = true
                }
            };

            // حفظ المصنف باستخدام خيارات HTML المكوّنة باستخدام معامل خيارات الحفظ
            workbook.Save("LowCodeHtmlExport.html", saveOptions.HtmlOptions);

            Console.WriteLine("HTML file saved successfully with low code options.");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptions](../lowcodesaveoptions/)
* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


