---
title: "LowCodeMergeOptions.LoadOptionsProvider"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية LowCodeMergeOptions. موفر خيارات الحفظ لتخزين الأجزاء المقسمة"
type: docs
url: /ar/net/aspose.cells.lowcode/lowcodemergeoptions/loadoptionsprovider/
---
## LowCodeMergeOptions.LoadOptionsProvider property

مزود خيارات الحفظ لحفظ الأجزاء المقسمة.

```csharp
public AbstractLowCodeLoadOptionsProvider LoadOptionsProvider { get; set; }
```

### ملاحظات

إذا تم تحديد هذه الخاصية، فإن [`LoadOptions`](../../../aspose.cells/loadoptions/) لن يكون له أي تأثير لأن مخرجات كل جزء مقسم سيتم تحديدها بواسطة الموفر.

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using Aspose.Cells.LowCode;
    using System;

    public class LowCodeMergeOptionsPropertyLoadOptionsProviderDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مثيل من LowCodeMergeOptions
            LowCodeMergeOptions mergeOptions = new LowCodeMergeOptions();

            // عرض القيمة الحالية لـ LoadOptionsProvider (يجب أن تكون null في البداية)
            Console.WriteLine("Current LoadOptionsProvider value: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // إنشاء تنفيذ مخصص لـ LoadOptionsProvider
            mergeOptions.LoadOptionsProvider = new CustomLoadOptionsProvider();

            // إظهار تعيين الخاصية
            Console.WriteLine("After setting LoadOptionsProvider: " + (mergeOptions.LoadOptionsProvider == null ? "null" : "not null"));

            // استخدام خيارات الدمج مع الموفر
            // عادةً ما يتم استخدام ذلك مع الأساليب التي تعالج ملفات متعددة
            // للتوضيح، سنتحقق فقط مما إذا كان الموفر يمكنه الانتقال إلى التالي
            bool hasNext = mergeOptions.LoadOptionsProvider.MoveNext();
            Console.WriteLine("LoadOptionsProvider MoveNext result: " + hasNext);

            // احفظ المصنف
            workbook.Save("PropertyLoadOptionsProviderDemo.xlsx");
        }

        private class CustomLoadOptionsProvider : AbstractLowCodeLoadOptionsProvider
        {
            private int counter = 0;
            private readonly LowCodeLoadOptions options = new LowCodeLoadOptions();

            public override LowCodeLoadOptions Current => options;

            public override bool MoveNext()
            {
                // محاكاة وجود 3 ملفات للمعالجة
                if (counter < 3)
                {
                    counter++;
                    return true;
                }
                return false;
            }

            public override void Finish(LowCodeLoadOptions part)
            {
                // منطق التنظيف أو الإنهاء سيُوضع هنا
            }
        }
    }
}
```

### انظر أيضًا

* class [AbstractLowCodeLoadOptionsProvider](../../abstractlowcodeloadoptionsprovider/)
* class [LowCodeMergeOptions](../)
* namespace [Aspose.Cells.LowCode](../../../aspose.cells.lowcode/)
* assembly [Aspose.Cells](../../../)


