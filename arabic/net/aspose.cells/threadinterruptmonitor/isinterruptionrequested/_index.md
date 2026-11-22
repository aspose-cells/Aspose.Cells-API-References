---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadInterruptMonitor. هذا التنفيذ يتحقق فقط مما إذا كان الوقت المستغرق من بدء هذا المراقب حتى الآن أكبر من الحد المحدد من قبل المستخدم"
type: docs
url: /ar/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

يتحقق هذا التنفيذ فقط مما إذا كانت تكلفة الوقت (من لحظة بدء هذا المراقب حتى الآن) أكبر من الحد المحدد من قبل المستخدم.

```csharp
public override bool IsInterruptionRequested { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;

    public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مثيل من ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // ابدأ المراقبة بحد 2 ثانية
            monitor.StartMonitor(2000);

            // محاكاة عملية طويلة الأمد
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // تحقق مما إذا تم طلب الانقطاع
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // محاكاة العمل
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // إنهاء المراقبة
            monitor.FinishMonitor();

            // حفظ النتيجة
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


