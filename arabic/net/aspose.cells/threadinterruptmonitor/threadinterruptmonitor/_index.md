---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "منشئ ThreadInterruptMonitor. ينشئ مراقب مقاطعة واحد"
type: docs
url: /ar/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

ينشئ مراقب انقطاع واحد.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // إنشاء دفتر عمل جديد
            Workbook workbook = new Workbook();
            
            // إنشاء ThreadInterruptMonitor مع تعيين throwOnInterrupted إلى false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // تعيين حد زمني قصير (100 مللي ثانية) للعرض
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // تنفيذ عملية طويلة (ستتم مقاطعتها)
                for (int i = 0; i < 100000; i++)
                {
                    workbook.Worksheets[0].Cells[i % 100, i / 100].PutValue(i);
                }
                
                Console.WriteLine("Operation completed without interruption");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### انظر أيضًا

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


