---
title: "الفئة AbstractLowCodeLoadOptionsProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "الفئة Aspose.Cells.LowCode.AbstractLowCodeLoadOptionsProvider. تنفيذ لتوفير خيارات تحميل متعددة للعمليات التي تستخدم مدخلات متعددة مثل ملفات القالب."
type: docs
url: /ar/net/aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/
---
## AbstractLowCodeLoadOptionsProvider class

تنفيذ لتوفير خيارات تحميل متعددة للعمليات التي تستخدم مدخلات متعددة (مثل ملفات القالب).

```csharp
public abstract class AbstractLowCodeLoadOptionsProvider
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| abstract [Current](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/current/) { get; } | يحصل على خيارات التحميل التي يتم منها تحميل بيانات الجزء المعالج حالياً. |

## الطرق

| الاسم | الوصف |
| --- | --- |
| virtual [Finish](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/finish/)(LowCodeLoadOptions) | يطلق الموارد بعد معالجة الجزء الحالي من الإدخال. |
| abstract [MoveNext](../../aspose.cells.lowcode/abstractlowcodeloadoptionsprovider/movenext/)() | يتحقق مما إذا كان هناك المزيد من الإدخال. |

### ملاحظات

على سبيل المثال، ميزة [`SpreadsheetMerger`](../spreadsheetmerger/) تتطلب ملفات قالب متعددة للدمج.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeClassAbstractLowCodeLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // إنشاء تنفيذ مخصص لـ AbstractLowCodeLoadOptionsProvider
            var provider = new CustomLoadOptionsProvider();

            // معالجة مدخلات متعددة باستخدام الموفر
            while (provider.MoveNext())
            {
                // الحصول على خيارات التحميل الحالية
                LowCodeLoadOptions currentOptions = provider.Current;
                Console.WriteLine($"Processing with load options: {currentOptions}");

                // إنشاء دفتر عمل باستخدام الخيارات الحالية
                Workbook workbook = new Workbook(FileFormatType.Xlsx);
                Worksheet worksheet = workbook.Worksheets[0];

                // عرض الاستخدام مع دفتر العمل
                worksheet.Cells["A1"].PutValue("Processed with custom provider");
                
                // إنهاء معالجة هذا الجزء
                provider.Finish(currentOptions);
            }
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int currentIndex = 0;
            private readonly LowCodeLoadOptions[] optionsList = new LowCodeLoadOptions[]
            {
                new LowCodeLoadOptions(),
                new LowCodeLoadOptions { InputFile = "protected.xlsx" }, // Password would be handled separately
                new LowCodeLoadOptions() // MemorySetting would be handled separately
            };

            public override LowCodeLoadOptions Current => optionsList[currentIndex];

            public override bool MoveNext()
            {
                if (currentIndex < optionsList.Length - 1)
                {
                    currentIndex++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // منطق التنظيف أو الإنهاء لكل جزء
                Console.WriteLine($"Finished processing part {currentIndex}");
            }
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells.LowCode](../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../)


