---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SystemTimeInterruptMonitor. هذا التنفيذ يتحقق فقط مما إذا كانت تكلفة الوقت من لحظة بدء هذا المراقب حتى الآن أكبر من الحد المحدد من قبل المستخدم"
type: docs
url: /ar/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من SystemTimeInterruptMonitor
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // بدء المراقبة بحد زمنى قدره 5 ثوانٍ
            monitor.StartMonitor(5000);

            // عرض القيمة الأولية لـ IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // محاكاة عملية طويلة الأمد
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // تحقق مما إذا تم طلب الانقطاع
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // عرض القيمة النهائية لـ IsInterruptionRequested
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // حفظ النتيجة
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


