---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة ThreadInterruptMonitor. يبدأ المراقب بالحد الزمني المحدد. وقت البدء لحساب الوقت المستغرق هو عندما يتم استدعاء هذه الطريقة فقط، لذا يجب بدء الإجراء الذي يحتاج إلى مراقبة مباشرة بعد هذا الاستدعاء"
type: docs
url: /ar/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

يبدأ المراقب بالحد الزمني المحدد. وقت البدء لحساب تكلفة الوقت هو لحظة استدعاء هذه الطريقة، لذا يجب بدء الإجراء الذي يحتاج إلى مراقبة مباشرةً بعد هذا الاستدعاء.

```csharp
public void StartMonitor(int msLimit)
```

| معامل | نوع | الوصف |
| --- | --- | --- |
| msLimit | Int32 | حد الوقت (مللي ثانية) لطلب الانقطاع. |

### أمثلة

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodStartMonitorWithInt32Demo
    {
        public static void Run()
        {
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            monitor.StartMonitor(1000);

            try
            {
                Workbook wb = new Workbook("Large.xlsx", lopts);
                monitor.FinishMonitor();

                monitor.StartMonitor(1500);
                wb.Save("result.xlsx");
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


