---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SystemTimeInterruptMonitor-konstruktor. Skapar en avbrottsmonitor"
type: docs
url: /sv/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

Skapar en avbrottsmonitor.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
```

| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Skapa en instans med terminateWithoutException satt till false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Ställ in laddningsalternativ med monitorn
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Starta övervakning med 1 sekunders tidsgräns
            monitor.StartMonitor(1000);

            try
            {
                // Försök att läsa in en arbetsbok
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // Återställ monitorn för sparoperation med 1,5 sekunders gräns
                monitor.StartMonitor(1500);
                wb.Save("output.xlsx");
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


