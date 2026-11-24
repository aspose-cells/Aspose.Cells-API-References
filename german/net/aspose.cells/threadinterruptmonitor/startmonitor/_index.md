---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadInterruptMonitor-Methode. Startet den Monitor mit dem angegebenen Zeitlimit. Der Startzeitpunkt zur Berechnung der Zeitkosten ist genau dann, wenn diese Methode aufgerufen wird, sodass das zu überwachende Verfahren unmittelbar nach diesem Aufruf gestartet werden sollte."
type: docs
url: /de/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

Startet den Monitor mit dem angegebenen Zeitlimit. Der Startzeitpunkt zur Berechnung der Zeitkosten ist genau der Moment, in dem diese Methode aufgerufen wird, sodass das zu überwachende Verfahren unmittelbar nach diesem Aufruf gestartet werden sollte.

```csharp
public void StartMonitor(int msLimit)
```

| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| msLimit | Int32 | Zeitlimit (ms), um die Unterbrechung zu erzwingen. |

### Beispiele

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

### Siehe auch

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


