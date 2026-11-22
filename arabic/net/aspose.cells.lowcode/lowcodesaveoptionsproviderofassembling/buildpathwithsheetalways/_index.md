---
title: "LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfAssembling. ما إذا كان يجب إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة لن يتم إضافة فهرس الورقة أو اسمها والبادئة المقابلة إلى مسار الملف."
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/buildpathwithsheetalways/
---
## LowCodeSaveOptionsProviderOfAssembling.BuildPathWithSheetAlways property

ما إذا كان يتم إضافة فهرس الورقة أو اسمها إلى مسار الملف دائمًا. القيمة الافتراضية هي false، أي عندما تكون هناك ورقة واحدة فقط، لن يتم إضافة فهرس الورقة (أو اسمها) والبادئة المقابلة إلى مسار الملف.

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

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyBuildPathWithSheetAlwaysDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد بورقة عمل واحدة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "DataSheet";
            
            // إنشاء نسخة من LowCodeSaveOptionsProviderOfAssembling
            LowCodeSaveOptionsProviderOfAssembling provider = new LowCodeSaveOptionsProviderOfAssembling();
            
            // تكوين إعدادات المسار
            provider.PathHeader = "output/";
            provider.PathTail = ".xlsx";
            provider.UseSheetName = true; // Use sheet name instead of index
            provider.SheetPrefix = "_Sheet_";
            provider.SplitPartPrefix = "_Part_";
            
            // عرض قيمة الخاصية الأولية
            Console.WriteLine("Initial BuildPathWithSheetAlways: " + provider.BuildPathWithSheetAlways);
            
            // عرض مسار الملف بدون BuildPathWithSheetAlways
            string defaultPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (default): " + defaultPath);
            
            // ضبط BuildPathWithSheetAlways إلى true
            provider.BuildPathWithSheetAlways = true;
            Console.WriteLine("\nAfter setting BuildPathWithSheetAlways to true: " + provider.BuildPathWithSheetAlways);
            
            // عرض مسار الملف مع BuildPathWithSheetAlways (حتى مع ورقة واحدة)
            string updatedPath = $"{provider.PathHeader}{provider.SheetPrefix}{worksheet.Name}{provider.SplitPartPrefix}0{provider.PathTail}";
            Console.WriteLine("Generated path (updated): " + updatedPath);
            
            // حفظ دفتر العمل (سيتبع سلوك التقسيم إعدادات الموفر في السيناريوهات الحقيقية)
            workbook.Save("BuildPathWithSheetAlwaysDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


