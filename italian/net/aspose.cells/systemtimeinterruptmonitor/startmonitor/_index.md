---
title: "SystemTimeInterruptMonitor.StartMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo SystemTimeInterruptMonitor. Avvia il monitor con il limite di tempo specificato. Il tempo di inizio per calcolare il costo temporale è proprio il momento in cui questo metodo viene chiamato, quindi la procedura che deve essere monitorata dovrebbe essere avviata subito dopo questa chiamata."
type: docs
url: /it/net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

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

### Vedi anche

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


