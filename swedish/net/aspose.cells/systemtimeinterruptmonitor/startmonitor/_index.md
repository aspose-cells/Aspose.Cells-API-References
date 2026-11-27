---
title: "SystemTimeInterruptMonitor.StartMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SystemTimeInterruptMonitor-metoden. Startar övervakaren med den angivna tidsgränsen. Starttiden för att beräkna tidskostnaden är precis när denna metod anropas, så proceduren som behöver övervakas bör startas omedelbart efter detta anrop."
type: docs
url: /sv/net/aspose.cells/systemtimeinterruptmonitor/startmonitor/
---
## SystemTimeInterruptMonitor.StartMonitor method

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

### Se även

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


