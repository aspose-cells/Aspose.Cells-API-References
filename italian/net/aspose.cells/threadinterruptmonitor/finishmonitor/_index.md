---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ThreadInterruptMonitor. Termina il monitor per una procedura"
type: docs
url: /it/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

Conclude il monitor per una procedura.

```csharp
public void FinishMonitor()
```

### Osservazioni

Chiamare questo metodo dopo la procedura monitorata può rilasciare il thread del monitor in anticipo, soprattutto quando non vi è alcuna interruzione (il tempo di esecuzione di quella procedura è inferiore al limite di tempo specificato).

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // Crea un'istanza di ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Creare LoadOptions e impostare InterruptMonitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Avviare il monitoraggio con timeout di 1 secondo
            monitor.StartMonitor(1000);

            try
            {
                // Simula un'operazione a lungo termine
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // Terminare il monitoraggio dell'operazione
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

### Vedi anche

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


