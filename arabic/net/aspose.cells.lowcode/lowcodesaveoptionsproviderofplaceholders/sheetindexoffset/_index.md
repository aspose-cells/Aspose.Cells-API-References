---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfPlaceHolders. إزاحة مؤشر أوراق العمل بين ما يُستخدم في مسار الملف والقيمة الفعلية لمؤشر الورقة"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexOffset property

إزاحة فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على عدة أوراق
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // إنشاء نسخة من LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheet_index}.xlsx";
            var optionsProvider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // عرض قيمة SheetIndexOffset الحالية (الافتراضية هي 0)
            Console.WriteLine("Current SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // تعيين SheetIndexOffset إلى 1 لتغيير مؤشرات الأوراق في أسماء ملفات الإخراج
            optionsProvider.SheetIndexOffset = 1;
            Console.WriteLine("New SheetIndexOffset value: " + optionsProvider.SheetIndexOffset);

            // تكوين خيارات الحفظ
            optionsProvider.SaveOptionsTemplate = new LowCodeSaveOptions();
            optionsProvider.SaveOptionsTemplate.SaveFormat = SaveFormat.Xlsx;

            // إظهار تأثير SheetIndexOffset على أسماء ملفات الإخراج
            // عادةً ما يتم استخدام هذا مع GetSaveOptions() أثناء عمليات الحفظ الفعلية
            Console.WriteLine("With SheetIndexOffset=1, output files would be named:");
            Console.WriteLine("Sheet1 -> output_1.xlsx (original index 0 + offset 1)");
            Console.WriteLine("Sheet2 -> output_2.xlsx (original index 1 + offset 1)");
            Console.WriteLine("Sheet3 -> output_3.xlsx (original index 2 + offset 1)");

            // إعادة الضبط إلى القيمة الافتراضية
            optionsProvider.SheetIndexOffset = 0;
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


