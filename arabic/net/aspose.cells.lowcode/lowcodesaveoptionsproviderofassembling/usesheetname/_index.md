---
title: "LowCodeSaveOptionsProviderOfAssembling.UseSheetName"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSaveOptionsProviderOfAssembling. ما إذا كان يبني مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. القيمة الافتراضية هي false"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesaveoptionsproviderofassembling/usesheetname/
---
## LowCodeSaveOptionsProviderOfAssembling.UseSheetName property

ما إذا كان يتم بناء مسار الملف باستخدام اسم الورقة بدلاً من فهرس الورقة. القيمة الافتراضية هي false.

```csharp
public bool UseSheetName { get; set; }
```

### ملاحظات

اسم الورقة لن يتم إعادة بنائه تلقائيًا أبدًا. لذا عند ضبطه على true، يرجى التأكد من عدم وجود اسم ورقة خاص يمكن أن يسبب مسار ملف أو اسم غير صالح.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSaveOptionsProviderOfAssemblingPropertyUseSheetNameDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد مع ورقة عمل مسماة
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Name = "MonthlyReport";
            
            // إضافة بيانات عينة لتوضيح عملية التقسيم
            for(int i = 0; i < 15; i++)
            {
                worksheet.Cells[$"A{i+1}"].PutValue($"Record {i+1}");
            }

            // إنشاء وتكوين الموفر
            var provider = new LowCodeSaveOptionsProviderOfAssembling
            {
                PathHeader = "split_files/",
                PathTail = ".xlsx",
                SheetPrefix = "Sheet_",
                SplitPartPrefix = "Part_",
                SaveOptionsTemplate = new LowCodeSaveOptions { SaveFormat = SaveFormat.Xlsx }
            };

            // إظهار UseSheetName=false (الافتراضي)
            Console.WriteLine($"Default UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_default", provider.SaveOptionsTemplate.SaveFormat);

            // تغيير الخاصية وإظهار السلوك الجديد
            provider.UseSheetName = true;
            Console.WriteLine($"\nModified UseSheetName: {provider.UseSheetName}");
            workbook.Save("output_modified", provider.SaveOptionsTemplate.SaveFormat);

            Console.WriteLine("Check 'split_files' directory for output files with different naming schemes");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptionsProviderOfAssembling](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


