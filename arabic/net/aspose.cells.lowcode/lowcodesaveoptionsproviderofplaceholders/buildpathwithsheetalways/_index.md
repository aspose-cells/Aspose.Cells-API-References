---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfPlaceHolders. ما إذا كان يجب إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة، لن يتم إضافة فهرس الورقة والاسم والبادئة المقابلة prefixSheetNamePrefix إلى مسار الملف"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSheetAlways property

ما إذا كان يجب إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة، لن يتم إضافة فهرس الورقة والاسم والبادئة المقابلة ([`SheetNamePrefix`](../sheetnameprefix/)) إلى مسار الملف.

```csharp
public bool BuildPathWithSheetAlways { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // إنشاء مصنف بورقتين لإظهار اختلافات المسار
            Workbook workbook = new Workbook();
            workbook.Worksheets.Add("Sheet2");
            
            // تكوين الموفر باستخدام عنصر نائب لفهرس الورقة
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Output_{sheet_index}.xlsx")
            {
                // إظهار إزاحة فهرس الورقة (اختياري)
                SheetIndexOffset = 1
            };

            Console.WriteLine($"Initial BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");

            // حفظ بفهرس الورقة فقط عند وجود أوراق متعددة (السلوك الافتراضي)
            provider.BuildPathWithSheetAlways = false;
            SaveWithProvider(workbook, provider, "DefaultBehavior");

            // فرض فهرس الورقة في أسماء الملفات حتى للأوراق المفردة
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine($"Modified BuildPathWithSheetAlways: {provider.BuildPathWithSheetAlways}");
            SaveWithProvider(workbook, provider, "ForcedSheetIndex");
        }

        private static void SaveWithProvider(Workbook workbook, LowCodeSaveOptionsProviderOfPlaceHolders provider, string saveDescription)
        {
            // تكوين خيارات الحفظ بتنسيق JSON لتمكين الانقسام
            var saveOptions = new LowCodeSaveOptions
            {
                SaveFormat = SaveFormat.Json
            };

            // تكوين الموفر مع خيارات الحفظ
            provider.SaveOptionsTemplate = saveOptions;

            // حفظ باستخدام المسارات التي يحددها الموفر
            Console.WriteLine($"Saving with {saveDescription} - check output files");
            workbook.Save($"dummy_{saveDescription}.json", saveOptions.SaveFormat);
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


