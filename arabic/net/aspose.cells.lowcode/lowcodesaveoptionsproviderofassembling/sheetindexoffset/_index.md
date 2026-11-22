---
title: "LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfAssembling. إزاحة فهرس الأوراق بين ما يُستخدم في مسار الملف والقيمة الفعلية SheetIndex"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/sheetindexoffset/
---
## LowCodeSaveOptionsProviderOfAssembling.SheetIndexOffset property

إزاحة فهرس الورقة بين ما يُستخدم في مسار الملف والقيمة الفعلية ([`SheetIndex`](../../splitpartinfo/sheetindex/)).

```csharp
public int SheetIndexOffset { get; set; }
```

### ملاحظات

يُطبق فقط عندما يكون [`UseSheetName`](../usesheetname/) false.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertySheetIndexOffsetDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد يحتوي على عدة أوراق
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("SalesData");
            workbook.Worksheets.Add("Inventory");

            // تهيئة موفر خيارات الحفظ
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "output/Quarter_",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet",
                SheetIndexOffset = 10,
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // عرض الإزاحة الأصلية
            Console.WriteLine($"Original SheetIndexOffset: {provider.SheetIndexOffset}");

            // حفظ مع الإزاحة الأولية (ستُرقم الأوراق 10 و 11)
            workbook.Save("output/with_offset", provider.SaveOptionsTemplate.SaveFormat);

            // غيّر الإزاحة واحفظ مرة أخرى
            provider.SheetIndexOffset = 100;
            Console.WriteLine($"Modified SheetIndexOffset: {provider.SheetIndexOffset}");
            
            // حفظ مع الإزاحة الجديدة (ستُرقم الأوراق 100 و 101)
            workbook.Save("output/with_modified_offset", provider.SaveOptionsTemplate.SaveFormat);
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


