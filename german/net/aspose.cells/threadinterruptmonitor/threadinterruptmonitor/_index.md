---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadInterruptMonitor-Konstruktor. Erstellt einen Unterbrechungsmonitor"
type: docs
url: /de/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Konstruiert einen Unterbrechungsmonitor.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Erstelle einen ThreadInterruptMonitor mit throwOnInterrupted auf false gesetzt
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // Setze ein kurzes Zeitlimit (100 ms) zur Demonstration
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // Führe eine lange Operation aus (wird unterbrochen)
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

### Siehe auch

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


