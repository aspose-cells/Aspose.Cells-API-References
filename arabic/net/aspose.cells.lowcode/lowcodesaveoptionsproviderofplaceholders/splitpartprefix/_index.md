---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfPlaceHolders. البادئة لمؤشر الجزء المقسم"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartPrefix property

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
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartPrefixDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            for (int i = 0; i < 25; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data row {i + 1}";
            }

            // تكوين قالب خيارات الحفظ
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();

            // تهيئة الموفر باستخدام عنصر نائب للجزء المقسم
            LowCodeSaveOptionsProviderOfPlaceHolders provider = new LowCodeSaveOptionsProviderOfPlaceHolders("SplitResult_Sheet{sheet}_Part{split}.xlsx")
            {
                SaveOptionsTemplate = saveOptionsTemplate
            };

            // عرض وتعديل SplitPartPrefix
            Console.WriteLine($"Initial SplitPartPrefix: {provider.SplitPartPrefix}");
            provider.SplitPartPrefix = "Section";
            Console.WriteLine($"Updated SplitPartPrefix: {provider.SplitPartPrefix}");

            // حفظ المصنف بأجزاء مقسمة باستخدام تنسيق الحفظ الخاص بالموفر
            workbook.Save("output", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'output' directory for split files with 'Section' prefix");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


