---
title: "فئة AbstractInterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "فئة Aspose.Cells.AbstractInterruptMonitor. مراقب لطلبات الإيقاف في جميع العمليات المستهلكة للوقت"
type: docs
url: /ar/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

مراقبة لطلبات الإيقاف في جميع العمليات المستهلكة للوقت.

```csharp
public abstract class AbstractInterruptMonitor
```

## الخصائص

| الاسم | الوصف |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | يشير إلى ما إذا كان تم طلب إيقاف العملية الحالية. إذا كان صحيحًا فسيتم إيقاف العملية الحالية. يجب على التنفيذ إجراء فحص سريع وفعال هنا، وإلا قد يصبح عنق زجاجة آخر للإجراء. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | عند انقطاع الإجراء، سواءً إنهاء الإجراء بهدوء أو إلقاء استثناء. القيمة الافتراضية هي false، أي عندما يكون [`IsInterruptionRequested`](./isinterruptionrequested/) true، سيتم إلقاء [`CellsException`](../cellsexception/) مع رمز Interrupted. |

### أمثلة

```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;

namespace AsposeCellsExamples
{
    // تنفيذ مخصص لـ AbstractInterruptMonitor
    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        //ملف النتيجة صحيح
        public override bool IsInterruptionRequested
        {
            get
            {
                Console.WriteLine("Get the return value of whether to interrupt the program===");
                // منطق لتحديد ما إذا كان الانقطاع مطلوبًا
                return false; // Change this based on your logic
            }
        }

        public override bool TerminateWithoutException
        {
            get => false; // Change this based on your logic
        }

        //// ملف النتيجة يتعطل
        //public override bool IsInterruptionRequested
        //{
        //    get
        //    {
        //        Console.WriteLine("احصل على قيمة الإرجاع لتحديد ما إذا كان يجب مقاطعة البرنامج===");
        //        // منطق لتحديد ما إذا كان الانقطاع مطلوبًا
        //        //return false; // غيّر هذا بناءً على منطقك
        //        return true;
        //    }
        //}

        //public override bool TerminateWithoutException
        //{
        //    get => true; // غيّر هذا بناءً على منطقك
        //}
    }

    public class InterruptMonitorDemo
    {
        public static void RunDemo()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // أضف بعض البيانات التجريبية
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // إنشاء مثيل من CustomInterruptMonitor
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // تعيين خيارات التحميل باستخدام مراقب الانقطاع المخصص
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // تحميل المصنف باستخدام الخيارات المحددة
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // إجراء الحسابات
            workbook.CalculateFormula();

            // احفظ المصنف
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


