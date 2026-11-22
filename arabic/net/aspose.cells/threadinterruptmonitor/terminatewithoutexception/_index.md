---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "خاصية ThreadInterruptMonitor. راجع TerminateWithoutException. يتم تحديد هذه الخاصية من قبل المستخدم عند إنشاء مثيل هذا المراقب"
type: docs
url: /ar/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

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

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // إنشاء مثيل من ThreadInterruptMonitor بقيمة مبدئية لـ TerminateWithoutException
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // عرض القيمة الحالية للخاصية
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // ابدأ المراقبة بحد 5 ثوانٍ
            monitor.StartMonitor(5000);

            // عرض معالجة قد يتم مقاطعتها
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // محاكاة معالجة طويلة
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Processing was interrupted");
                        break;
                    }
                    worksheet.Cells[i, 0].Value = "Value " + i;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception occurred: " + ex.Message);
            }
            finally
            {
                monitor.FinishMonitor();
            }

            // إنشاء مراقب آخر مع تعيين TerminateWithoutException إلى true
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // حفظ النتيجة
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### انظر أيضًا

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


