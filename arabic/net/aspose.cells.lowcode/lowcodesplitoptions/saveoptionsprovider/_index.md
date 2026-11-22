---
title: "LowCodeSplitOptions.SaveOptionsProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeSplitOptions. موفر خيارات الحفظ لحفظ الأجزاء المقسمة"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/
---
## LowCodeSplitOptions.SaveOptionsProvider property

مزود خيارات الحفظ لحفظ الأجزاء المقسمة.

```csharp
public AbstractLowCodeSaveOptionsProvider SaveOptionsProvider { get; set; }
```

### ملاحظات

إذا تم تحديد هذه الخاصية، [`SaveOptions`](../saveoptions/) لن تكون لها أي تأثير لأن مخرجات كل جزء مقسم سيتم تحديدها بواسطة الموفر.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeSplitOptionsPropertySaveOptionsProviderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // املأ بعض بيانات العينة
            worksheet.Cells["A1"].PutValue("Name");
            worksheet.Cells["B1"].PutValue("Value");
            worksheet.Cells["A2"].PutValue("Item1");
            worksheet.Cells["B2"].PutValue(100);
            worksheet.Cells["A3"].PutValue("Item2");
            worksheet.Cells["B3"].PutValue(200);
            
            // إنشاء نسخة من LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // عرض قيمة SaveOptionsProvider الحالية (null بشكل افتراضي)
            Console.WriteLine("Current SaveOptionsProvider value: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // إنشاء SaveOptionsProvider مخصص
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // إظهار تأثير تعيين SaveOptionsProvider
            // في سيناريو واقعي، سيُستخدم هذا عند تقسيم الملفات
            Console.WriteLine("After setting SaveOptionsProvider: " + (splitOptions.SaveOptionsProvider == null ? "null" : "not null"));
            
            // حفظ المصنف (على الرغم من عدم توضيح التقسيم هنا)
            workbook.Save("PropertySaveOptionsProviderDemo.xlsx");
        }
    }

    // تنفيذ مخصص لـ AbstractLowCodeSaveOptionsProvider
    public class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
    {
        public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo part)
        {
            // إنشاء خيارات حفظ مخصصة لكل جزء مقسم
            LowCodeSaveOptions options = new LowCodeSaveOptions();
            options.SaveFormat = SaveFormat.Xlsx;
            return options;
        }

        public override void Finish(LowCodeSaveOptions part)
        {
            // إجراء أي تنظيف بعد حفظ كل جزء
            Console.WriteLine("Finished saving part");
        }
    }
}
```

### انظر أيضًا

* class [AbstractLowCodeSaveOptionsProvider](../../abstractlowcodesaveoptionsprovider/)
* class [LowCodeSplitOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


