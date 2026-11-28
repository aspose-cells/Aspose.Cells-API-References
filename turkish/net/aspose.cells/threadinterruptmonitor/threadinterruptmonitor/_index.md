---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "Aspose.Cells için .NET API Referansı"
description: "ThreadInterruptMonitor yapıcı. Bir kesinti izleyicisi oluşturur"
type: docs
url: /tr/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Bir kesinti izleyicisi oluşturur.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Parametre | Tür | Açıklama |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Örnekler

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Yeni bir çalışma kitabı oluştur
            Workbook workbook = new Workbook();
            
            // throwOnInterrupted özelliği false olarak ayarlanmış bir ThreadInterruptMonitor oluştur
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // Demonstrasyon için kısa bir zaman sınırı (100ms) ayarla
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // Uzun bir işlem gerçekleştir (kesintiye uğrayacak)
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

### Ayrıca Bakınız

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


