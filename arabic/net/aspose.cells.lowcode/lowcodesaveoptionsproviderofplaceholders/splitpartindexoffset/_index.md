---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfPlaceHolders. إزاحة فهرس أجزاء الانقسام بين ما يُستخدم في مسار الملف والقيمة الفعلية valuePartIndex"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SplitPartIndexOffset property

إزاحة فهرس الجزء المقسّم بين ما يُستخدم في مسار الملف والقيمة الفعلية له ([`PartIndex`](../../splitpartinfo/partindex/)).

```csharp
public int SplitPartIndexOffset { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySplitPartIndexOffsetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع بيانات عينة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 15; i++)
            {
                worksheet.Cells[i, 0].Value = $"Data Row {i + 1}";
            }

            // إنشاء قالب خيارات حفظ منخفض الكود
            LowCodeSaveOptions saveOptionsTemplate = new LowCodeSaveOptions();
            saveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // تهيئة الموفر باستخدام قالب المسار
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("output/SplitPart_{0}.xlsx");
            provider.SaveOptionsTemplate = saveOptionsTemplate;

            // عرض وتعديل SplitPartIndexOffset
            Console.WriteLine("Initial SplitPartIndexOffset: " + provider.SplitPartIndexOffset);
            provider.SplitPartIndexOffset = 1;

            // حفظ المصنف لإنشاء أجزاء مقسمة بفهرس معدل
            workbook.Save("SplitPartIndexOffsetDemo", saveOptionsTemplate.SaveFormat);

            Console.WriteLine("Generated split parts with offset applied.");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


