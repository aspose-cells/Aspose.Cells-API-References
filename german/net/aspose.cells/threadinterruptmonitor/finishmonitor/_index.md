---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "ThreadInterruptMonitor-Methode. Beendet den Monitor für ein Verfahren"
type: docs
url: /de/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

Beendet den Monitor für einen Vorgang.

```csharp
public void FinishMonitor()
```

### Hinweise

Der Aufruf dieser Methode nach dem überwachten Verfahren kann den Monitor-Thread früher freigeben, insbesondere wenn es dafür keine Unterbrechung gibt (die Zeitkosten dieses Verfahrens sind kleiner als das angegebene Zeitlimit).

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // Eine Instanz von ThreadInterruptMonitor erstellen
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // LoadOptions erstellen und den InterruptMonitor setzen
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Überwachung starten mit einem 1‑Sekunden‑Timeout
            monitor.StartMonitor(1000);

            try
            {
                // Eine langlaufende Operation simulieren
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // Überwachung des Vorgangs beenden
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

### Siehe auch

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


