---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadInterruptMonitor yöntemi. Belirtilen zaman sınırıyla izleyiciyi başlatır. Zaman maliyetini hesaplamak için başlangıç zamanı, bu yöntemin çağrıldığı an olur; bu nedenle izlenmesi gereken prosedür bu çağrının hemen ardından başlatılmalıdır"
type: docs
url: /tr/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

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

### Ayrıca Bakınız

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


