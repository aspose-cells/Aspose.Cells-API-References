---
title: "LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfAssembling. إزاحة فهرس الأجزاء المقسمة بين ما يُستخدم في مسار الملف والقيمة الفعلية للـ PartIndex"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/splitpartindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SplitPartIndexOffset property

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

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySplitPartIndexOffsetDemo
    {
        public static void Run()
        {
            // إنشاء مصنف ببيانات اختبار
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء ورقة العمل لإنشاء عدة أجزاء مقسمة
            for(int i = 0; i < 150; i++)
            {
                worksheet.Cells[$"A{i+1}"].Value = $"Item {i+1}";
            }

            // تكوين فواصل الصفحات لتقسيم إلى 3 أجزاء
            worksheet.HorizontalPageBreaks.Add(0, 50);
            worksheet.HorizontalPageBreaks.Add(0, 100);

            // إنشاء موفر وتكوين خيارات الحفظ
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Part_",
                SplitPartPrefix = "-",
                PathTail = ".xlsx",
                SplitPartIndexOffset = 10
            };

            // عرض التكوين الأولي
            Console.WriteLine($"Initial SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("First save operation (offset 10):");
            Console.WriteLine($"Expected filenames: output/Part_-10.xlsx, output/Part_-11.xlsx, output/Part_-12.xlsx");

            // غيّر الإزاحة وأظهر التكوين الجديد
            provider.SplitPartIndexOffset = 0;
            Console.WriteLine($"\nModified SplitPartIndexOffset: {provider.SplitPartIndexOffset}");
            Console.WriteLine("Second save operation (offset 0):");
            Console.WriteLine($"Expected filenames: output/Part_-0.xlsx, output/Part_-1.xlsx, output/Part_-2.xlsx");

            // عادةً ما تكون عملية الحفظ الفعلية:
            // workbook.Save("output/main.xlsx", new OoxmlSaveOptions { SaveProvider = provider });
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


