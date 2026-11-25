---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo ThreadInterruptMonitor. Avvia il monitor con il limite di tempo specificato. Il tempo di inizio per calcolare il tempo trascorso è proprio quando questo metodo viene chiamato, quindi la procedura da monitorare dovrebbe essere avviata subito dopo questa chiamata"
type: docs
url: /it/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

Avvia il monitor con il limite di tempo specificato. Il tempo di inizio per calcolare il tempo impiegato è proprio quando questo metodo viene chiamato, quindi la procedura da monitorare dovrebbe iniziare subito dopo questa chiamata.

```csharp
public void StartMonitor(int msLimit)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| msLimit | Int32 | limite di tempo (ms) per richiedere l'interruzione. |

### Esempi

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

### Vedi anche

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


