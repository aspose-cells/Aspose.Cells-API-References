---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfPlaceHolders. البادئة لمؤشر ورقة العمل"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/sheetnameprefix/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.SheetNamePrefix property

بادئة لفهرس ورقة العمل.

```csharp
public string SheetNamePrefix { get; set; }
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

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertySheetNamePrefixDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد يحتوي على ورقتي عمل
            Workbook workbook = new Workbook();
            workbook.Worksheets[0].Name = "SalesData";
            workbook.Worksheets.Add("FinancialReport");

            // تهيئة الموفر باستخدام قالب مسار يحتوي على عنصر نائب للورقة
            string pathTemplate = "output_{sheet}.xlsx";
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders(pathTemplate);

            // عرض قيمة SheetNamePrefix الأولية (فارغة بشكل افتراضي)
            Console.WriteLine("Initial SheetNamePrefix: " + provider.SheetNamePrefix);

            // تعيين بادئة جديدة وضمان أن توليد المسار يتضمن معلومات الورقة
            provider.SheetNamePrefix = "Q4_";
            provider.BuildPathWithSheetAlways = true;

            // تكوين خيارات الحفظ بالتنسيق الصحيح
            provider.SaveOptionsTemplate = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Xlsx // Set the correct save format
            };

            // حفظ المصنف باستخدام الموفر - يولد "output_Q4_SalesData.xlsx" و "output_Q4_FinancialReport.xlsx"
            workbook.Save("result_directory", SaveFormat.Xlsx); // Pass correct SaveFormat
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


