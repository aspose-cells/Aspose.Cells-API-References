---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية SystemTimeInterruptMonitor. راجع TerminateWithoutException. يتم تحديد هذه الخاصية من قبل المستخدم عند إنشاء نسخة هذا المراقب"
type: docs
url: /ar/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

انظر [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). يتم تحديد هذه الخاصية من قبل المستخدم عند إنشاء نسخة هذا المراقب.

```csharp
public override bool TerminateWithoutException { get; }
```

### أمثلة

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء نسخة من SystemTimeInterruptMonitor مع القيمة الأولية لخاصية TerminateWithoutException
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // عرض القيمة الحالية لخاصية TerminateWithoutException
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // بدء المراقبة بحد زمني قدره 1000 مللي ثانية
            monitor.StartMonitor(1000);

            // إظهار تأثير TerminateWithoutException من خلال محاولة عملية طويلة
            try
            {
                // محاكاة عملية طويلة قد تتجاوز الحد الزمني
                for (int i = 0; i < 100000; i++)
                {
                    worksheet.Cells[i, 0].Value = i;
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Operation interrupted by monitor");
                        break;
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception caught: " + ex.Message);
            }

            // إنشاء مراقب آخر مع تعيين TerminateWithoutException إلى true
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // احفظ المصنف
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


