---
title: "الفئة LowCodeSplitOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "Aspose.Cells.LowCode.LowCodeSplitOptions فئة. خيارات لتقسيم جدول البيانات"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodesplitoptions/
---
## LowCodeSplitOptions class

خيارات تقسيم جدول البيانات.

```csharp
public class LowCodeSplitOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodeSplitOptions](lowcodesplitoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [LoadOptions](../../aspose.cells.lowcode/lowcodesplitoptions/loadoptions/) { get; set; } | خيارات التحميل لتحميل جدول البيانات الذي سيتم تقسيمه. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptions/) { get; set; } | خيارات الحفظ لحفظ الأجزاء المقسمة. |
| [SaveOptionsProvider](../../aspose.cells.lowcode/lowcodesplitoptions/saveoptionsprovider/) { get; set; } | مزود خيارات الحفظ لحفظ الأجزاء المقسمة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeSplitOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];
            
            // ملء ورقة العمل ببيانات نموذجية
            worksheet.Cells["A1"].PutValue("Sample Data for Splitting");
            
            // إنشاء كائن من LowCodeSplitOptions
            LowCodeSplitOptions splitOptions = new LowCodeSplitOptions();
            
            // تكوين LoadOptions (مثال: معالجة المصدر المحمي بكلمة مرور)
            splitOptions.LoadOptions = new LowCodeLoadOptions();
            
            // تكوين SaveOptions (مثال: تعيين تنسيق الإخراج الافتراضي)
            splitOptions.SaveOptions = new LowCodeSaveOptions();
            
            // تنفيذ موفر SaveOptions مخصص لإعدادات الإخراج الديناميكية
            splitOptions.SaveOptionsProvider = new CustomSaveOptionsProvider();
            
            // مثال على التكامل: تقسيم workbook إلى أجزاء باستخدام الخيارات المكوَّنة
            // (افترض وجود طريقة مثل LowCodeEngine.Split(workbook, splitOptions, \"outputDir\"))
            // LowCodeEngine.Split(workbook, splitOptions, \"OutputDirectory\");
            
            // احفظ المصنف الأصلي للعرض
            workbook.Save("LowCodeSplitOptionsDemo.xlsx");
        }

        // تنفيذ مخصص لـ SaveOptionsProvider
        private class CustomSaveOptionsProvider : AbstractLowCodeSaveOptionsProvider
        {
            public override LowCodeSaveOptions GetSaveOptions(SplitPartInfo partInfo)
            {
                // منطق مثال: تبديل الإعدادات بناءً على فهرس التقسيم
                return new LowCodeSaveOptions();
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


