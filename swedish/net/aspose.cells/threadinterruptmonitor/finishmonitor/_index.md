---
title: "ThreadInterruptMonitor.FinishMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadInterruptMonitor metod. Avslutar monitorn för en procedur"
type: docs
url: /sv/net/aspose.cells/threadinterruptmonitor/finishmonitor/
---
## ThreadInterruptMonitor.FinishMonitor method

Avslutar övervakaren för ett förfarande.

```csharp
public void FinishMonitor()
```

### Anmärkningar

Att anropa denna metod efter den övervakade proceduren kan frigöra monitortråden tidigare, särskilt när det inte finns någon avbrott för den (tidskostnaden för den proceduren är mindre än den angivna tidsgränsen).

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class ThreadInterruptMonitorMethodFinishMonitorDemo
    {
        public static void Run()
        {
            // Skapa en instans av ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Skapa LoadOptions och sätt InterruptMonitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Starta övervakning med 1 sekunders timeout
            monitor.StartMonitor(1000);

            try
            {
                // Simulera en långvarig operation
                for (int i = 0; i < 5; i++)
                {
                    System.Threading.Thread.Sleep(200);
                    Console.WriteLine($"Processing step {i + 1}");
                }

                // Avsluta övervakning av operationen
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

### Se även

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


