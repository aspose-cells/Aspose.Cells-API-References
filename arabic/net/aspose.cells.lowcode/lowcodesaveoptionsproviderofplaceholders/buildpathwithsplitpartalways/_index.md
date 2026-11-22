---
title: "LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfPlaceHolders. ما إذا كان يجب إضافة فهرس جزء الانقسام إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء انقسام واحد، لن يتم إضافة فهرس جزء الانقسام والبادئة المقابلة prefixSplitPartPrefix إلى مسار الملف"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofplaceholders/buildpathwithsplitpartalways/
---
## LowCodeSaveOptionsProviderOfPlaceHolders.BuildPathWithSplitPartAlways property

ما إذا كان يجب إضافة فهرس جزء الانقسام إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما يكون هناك جزء انقسام واحد، لن يتم إضافة فهرس جزء الانقسام والبادئة المقابلة ([`SplitPartPrefix`](../splitpartprefix/)) إلى مسار الملف.

```csharp
public bool BuildPathWithSplitPartAlways { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfPlaceHoldersPropertyBuildPathWithSplitPartAlwaysDemo
    {
        public static void Run()
        {
            // إنشاء مصنف ببيانات لن يتم تقسيمها إلى أجزاء متعددة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].Value = "Single Part Demonstration";

            // إنشاء موفر باستخدام قالب المسار وشروط الانقسام التي تؤدي إلى جزء واحد
            var provider = new LowCodeSaveOptionsProviderOfPlaceHolders("Result_{split}.xlsx")
            {
                SaveOptionsTemplate = new LowCodeSaveOptions()
            };

            // إظهار حالة الخاصية false (الافتراضية)
            Console.WriteLine($"Initial BuildPathWithSplitPartAlways: {provider.BuildPathWithSplitPartAlways}");
            provider.BuildPathWithSplitPartAlways = false;
            
            // سيؤدي ذلك إلى إنشاء Result.xlsx عندما يكون هناك جزء واحد فقط
            Console.WriteLine("Saving with BuildPathWithSplitPartAlways=false");
            ExecuteDummySave(workbook, "Result.xlsx");

            // تبديل الخاصية وإظهار الحالة true
            provider.BuildPathWithSplitPartAlways = true;
            Console.WriteLine("\nSaving with BuildPathWithSplitPartAlways=true");
            
            // سيؤدي ذلك إلى إنشاء Result_0.xlsx حتى مع وجود جزء واحد
            ExecuteDummySave(workbook, "Result_0.xlsx");
        }

        private static void ExecuteDummySave(Workbook workbook, string filename)
        {
            // في الاستخدام الفعلي، استبدل بعملية حفظ تعتمد على الموفر
            Console.WriteLine($"Simulated save operation -> Filename: {filename}");
            workbook.Save(filename, SaveFormat.Xlsx);
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfPlaceHolders](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


