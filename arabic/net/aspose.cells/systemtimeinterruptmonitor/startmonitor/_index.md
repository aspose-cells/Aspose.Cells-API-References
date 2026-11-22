---
title: "SystemTimeInterruptMonitor.StartMonitor"
second_title: "مرجع API لـ Aspose.Cells لـ .NET"
description: "طريقة SystemTimeInterruptMonitor. يبدأ المراقب بالحد الزمني المحدد. وقت البدء لحساب تكلفة الوقت هو لحظة استدعاء هذه الطريقة، لذا يجب بدء الإجراء الذي يحتاج إلى مراقبة مباشرة بعد هذا الاستدعاء"
type: docs
url: /ar/net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

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
    public class SystemTimeInterruptMonitorMethodStartMonitorWithInt32Demo
    {
        public static void Run()
        {
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            monitor.StartMonitor(1000); // 1 second time limit

            try
            {
                Workbook wb = new Workbook("Large.xlsx", lopts);
                monitor.StartMonitor(1500); // 1.5 second time limit
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### انظر أيضًا

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


