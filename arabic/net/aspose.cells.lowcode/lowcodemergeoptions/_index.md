---
title: "الفئة LowCodeMergeOptions"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LowCode.LowCodeMergeOptions. خيارات دمج ملفات القالب المتعددة في ملف واحد"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodemergeoptions/
---
## LowCodeMergeOptions class

خيارات دمج ملفات القالب المتعددة في ملف واحد.

```csharp
public class LowCodeMergeOptions
```

## المنشئات

| الاسم | الوصف |
| --- | --- |
| [LowCodeMergeOptions](lowcodemergeoptions/)() | البناء الافتراضي. |

## الخصائص

| الاسم | الوصف |
| --- | --- |
| [LoadOptionsProvider](../../aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/) { get; set; } | مزود خيارات الحفظ لحفظ الأجزاء المقسمة. |
| [SaveOptions](../../aspose.cells.lowcode/lowcodemergeoptions/saveoptions/) { get; set; } | خيارات الحفظ لحفظ الأجزاء المقسمة. |

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassLowCodeMergeOptionsDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء وتكوين LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();
            
            // تعيين خيارات الحفظ لتنسيق الإخراج
            mergeOptions.SaveOptions = new LowCodeSaveOptions();
            
            // تعيين موفر خيارات التحميل المخصص
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();
            
            // مثال على التكامل (استخدام افتراضي مع وظيفة الدمج)
            // عادةً ما يتم استدعاؤه مع مسارات الملفات الفعلية
            // Workbook.Merge(new string[] { "template1.xlsx", "template2.xlsx" }, mergeOptions);
            
            // حفظ المصنف (لأغراض العرض)
            workbook.Save("LowCodeMergeOptionsDemo.xlsx");
        }
    }

    // موفر مخصص ينفذ الفئة المجردة
    public class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
    {
        public override bool MoveNext()
        {
            // تنفيذ بسيط لتلبية متطلبات الفئة المجردة
            return false;
        }

        public override LowCodeLoadOptions Current
        {
            get { throw new InvalidOperationException(); }
        }

        public LoadOptions GetLoadOptions(string fileName)
        {
            if (fileName.EndsWith(".xlsx", StringComparison.OrdinalIgnoreCase))
            {
                return new LoadOptions(LoadFormat.Xlsx);
            }
            return new LoadOptions();
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


