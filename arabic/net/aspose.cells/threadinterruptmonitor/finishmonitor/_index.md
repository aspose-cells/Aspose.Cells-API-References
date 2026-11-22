---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ThreadInterruptMonitor. تنهي المراقب لإجراء واحد"
type: docs
url: /ar/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

ينهي المراقب لإجراء واحد.

```csharp
public void FinishMonitor()
```

### ملاحظات

استدعاء هذه الطريقة بعد الإجراء المراقب يمكن أن يحرر خيط المراقبة مبكرًا، خاصةً عندما لا يكون هناك مقاطعة له (تكلفة الوقت لهذا الإجراء أقل من الحد الزمني المحدد).

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // إنشاء مثيل من ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // إنشاء LoadOptions وتعيين InterruptMonitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // بدء المراقبة بمهلة ثانية واحدة
            monitor.StartMonitor(1000);

            try
            {
                // محاكاة عملية طويلة الأمد
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // إنهاء مراقبة العملية
                monitor.FinishMonitor();
                Console.WriteLine("Operation completed successfully");
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


