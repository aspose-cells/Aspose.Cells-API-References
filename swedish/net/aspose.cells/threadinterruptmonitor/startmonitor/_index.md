---
title: "ThreadInterruptMonitor.StartMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadInterruptMonitor metod. Startar monitorn med den angivna tidsgränsen. Starttiden för att beräkna tidskostnaden är precis när denna metod anropas, så proceduren som ska övervakas bör startas omedelbart efter detta anrop."
type: docs
url: /sv/net/aspose.cells/threadinterruptmonitor/startmonitor/
---
## ThreadInterruptMonitor.StartMonitor method

Startar monitorn med den angivna tidsgränsen. Starttiden för att beräkna tidskostnaden är exakt när denna metod anropas, så proceduren som ska övervakas bör startas omedelbart efter detta anrop.

```csharp
public void StartMonitor(int msLimit)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| msLimit | Int32 | tidsgräns (ms) för att kräva avbrottet. |

### Exempel

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

### Se även

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


