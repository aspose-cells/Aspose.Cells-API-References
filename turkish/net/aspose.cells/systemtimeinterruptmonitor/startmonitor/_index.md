---
title: "SystemTimeInterruptMonitor.StartMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "SystemTimeInterruptMonitor yöntemi. Belirtilen zaman sınırlamasıyla monitörü başlatır. Zaman maliyetini hesaplamak için başlangıç zamanı, bu yöntemin çağrıldığı an olur; bu yüzden izlenmesi gereken prosedür bu çağrının hemen ardından başlatılmalıdır."
type: docs
url: /tr/net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

İzleyiciyi belirtilen zaman sınırıyla başlatır. Zaman maliyetini hesaplamak için başlangıç zamanı, bu yöntemin çağrıldığı zamandır, bu yüzden izlenmesi gereken prosedür bu çağrının hemen ardından başlatılmalıdır.

```csharp
public void StartMonitor(int msLimit)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| msLimit | Int32 | kesintiyi gerektirecek zaman sınırlaması (ms). |

### Örnekler

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

### Ayrıca Bakınız

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


