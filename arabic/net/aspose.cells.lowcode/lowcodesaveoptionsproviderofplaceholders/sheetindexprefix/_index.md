---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfPlaceHolders. البادئة لمؤشر ورقة العمل"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetindexprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetIndexPrefix property

بادئة لفهرس ورقة العمل.

```csharp
public string SheetIndexPrefix { get; set; }
```

### ملاحظات

إذا كان هناك ورقة عمل واحدة فقط وكان [`BuildPathWithSheetAlways`](../buildpathwithsheetalways/) غير صحيح، فلن تتم إضافة هذه البادئة وفهرس الورقة (أو اسمها) إلى مسار الملف الناتج.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetIndexPrefixDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع عدة أوراق عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            workbook.Worksheets.Add("Sheet3");

            // إنشاء نسخة من LowCodeSaveOptionsProviderOfPlaceHolders
            string pathTemplate = "output_{sheetindex}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // عرض وتعديل SheetIndexPrefix
            Console.WriteLine("Original SheetIndexPrefix: " + provider.SheetIndexPrefix);
            provider.SheetIndexPrefix = "sheet_";
            Console.WriteLine("Modified SheetIndexPrefix: " + provider.SheetIndexPrefix);

            // اضبط الخصائص المطلوبة الأخرى
            provider.BuildPathWithSheetAlways = true;
            provider.SaveOptionsTemplate = new LowCodeSaveOptions();

            // إظهار تأثير SheetIndexPrefix على مسارات الملفات
            foreach (Worksheet sheet in workbook.Worksheets)
            {
                // نظرًا لأننا لا نستطيع إنشاء وتعبئة SplitPartInfo مباشرةً،
                // سنقوم فقط بإظهار نمط التسمية دونه
                Console.WriteLine($"Sheet {sheet.Name} would save to: output_{provider.SheetIndexPrefix}{sheet.Index}.xlsx");
            }

            // احفظ المصنف لإظهار نمط التسمية
            workbook.Save("output_sheet_0.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


