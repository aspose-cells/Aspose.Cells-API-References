---
title: "LowCodeSplitOptions.SaveOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSplitOptions. خيارات الحفظ لحفظ الأجزاء المقسمة"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptions/
---
## LowCodeSplitOptions.SaveOptions property

خيارات الحفظ لحفظ الأجزاء المقسمة.

```csharp
public LowCodeSaveOptions SaveOptions { get; set; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsDemo
    {
        public static void Run()
        {
            // إنشاء مصنف جديد وإضافة بيانات نموذجية
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");

            // إنشاء كائن من LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();

            // عرض قيمة SaveOptions الأولية (null بشكل افتراضي)
            Console.WriteLine("Initial SaveOptions value: " + (splitOptions.SaveOptions == null ? "null" : splitOptions.SaveOptions.ToString()));

            // إنشاء وتكوين LowCodeSaveOptions لتنسيق PDF
            LowCodeSaveOptions pdfSaveOptions = new LowCodeSaveOptions();
            pdfSaveOptions.SaveFormat = SaveFormat.Pdf;

            // تعيين خيارات الحفظ إلى SplitOptions
            splitOptions.SaveOptions = pdfSaveOptions;

            // عرض قيمة SaveOptions المحدثة
            Console.WriteLine("Updated SaveOptions SaveFormat: " + splitOptions.SaveOptions.SaveFormat);

            // سيناريو استخدام مثال: تقسيم المصنف سيحفظ الأجزاء كملفات PDF
            // (سيعتمد كود التقسيم الفعلي على تنفيذ واجهة برمجة تطبيقات Aspose.Cells.LowCode)
            // LowCodeEngine.Split(workbook, splitOptions, "output_directory/");
            
            // احفظ المصنف الأصلي للعرض (ليس متأثراً بـ SplitOptions)
            workbook.Save("LowCodeSplitOptionsPropertySaveOptionsDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [LowCodeSaveOptions](../../lowcodesaveoptions/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


