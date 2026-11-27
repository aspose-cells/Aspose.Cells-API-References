---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadInterruptMonitor konstruktor. Konstruerar en avbrottsmonitor"
type: docs
url: /sv/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Skapar en avbrottsmonitor.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Skapa en ThreadInterruptMonitor med throwOnInterrupted satt till false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // Ställ in en kort tidsgräns (100ms) för demonstration
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // Utför en lång operation (kommer att avbrytas)
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

### Se även

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


