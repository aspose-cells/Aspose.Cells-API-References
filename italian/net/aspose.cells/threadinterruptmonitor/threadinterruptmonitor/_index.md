---
title: "ThreadInterruptMonitor.ThreadInterruptMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore ThreadInterruptMonitor. Costruisce un monitor di interruzione"
type: docs
url: /it/net/aspose.cells/threadinterruptmonitor/threadinterruptmonitor/
---
## ThreadInterruptMonitor constructor

Costruisce un monitor di interruzione.

```csharp
public ThreadInterruptMonitor(bool terminateWithoutException)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Creare un ThreadInterruptMonitor con throwOnInterrupted impostato a false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            workbook.InterruptMonitor = monitor;
            
            // Impostare un breve limite di tempo (100 ms) per la dimostrazione
            int timeLimit = 100;
            monitor.StartMonitor(timeLimit);

            try
            {
                // Eseguire un'operazione lunga (verrà interrotta)
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

### Vedi anche

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


