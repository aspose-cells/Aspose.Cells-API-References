---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfAssembling. بادئة لفهرس الجزء المقسّم"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartPrefix property

بادئة لفهرس الجزء المقسم.

```csharp
public string SplitPartPrefix { get; set; }
```

### ملاحظات

إذا كان هناك جزء مقسّم واحد فقط وكان [`BuildPathWithSplitPartAlways`](../buildpathwithsplitpartalways/) false، فلن تُضاف هذه البادئة وفهرس الجزء المقسّم (0) إلى مسار الملف الناتج.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using Aspose.Cells.Rendering;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل ببيانات تمتد عبر صفحات متعددة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 100; i++)
                worksheet.Cells[$"A{i + 1}"].Value = $"Data Row {i + 1}";

            // تكوين إعدادات الصفحة لإنشاء صفحات متعددة
            worksheet.PageSetup.PrintArea = "A1:A30";
            worksheet.PageSetup.FitToPagesTall = 1;

            // تهيئة موفر خيارات الحفظ مع تكوين التقسيم
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "SplitResults/",
                SplitPartPrefix = "OriginalPart_",
                PathTail = ".pdf",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Pdf }
            };

            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");

            // احفظ باستخدام البادئة الأولية (سيتم إنشاء SplitResults/OriginalPart_0.pdf إلخ.)
            workbook.Save("InitialSplit.pdf", new PdfSaveOptions());

            // تعديل بادئة التقسيم
            provider.SplitPartPrefix = "ModifiedPart_";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // احفظ باستخدام البادئة المعدلة (سيتم إنشاء SplitResults/ModifiedPart_0.pdf إلخ.)
            workbook.Save("ModifiedSplit.pdf", new PdfSaveOptions());
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


