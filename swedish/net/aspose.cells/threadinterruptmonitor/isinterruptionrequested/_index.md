---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadInterruptMonitor egenskap. Denna implementation kontrollerar bara om tidskostnaden från det att monitorn startades till nu är större än den av användaren angivna gränsen"
type: docs
url: /sv/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

Denna implementering kontrollerar bara om tidskostnaden (från det att monitorn startades till nu) är större än den användarspecificerade gränsen.

```csharp
public override bool IsInterruptionRequested { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;

    public class ThreadInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // Starta övervakning med en 2 sekunders gräns
            monitor.StartMonitor(2000);

            // Simulera en långvarig operation
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // Kontrollera om avbrott begärdes
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // Simulera arbete
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // Avsluta övervakning
            monitor.FinishMonitor();

            // Spara resultatet
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


