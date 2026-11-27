---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SystemTimeInterruptMonitor-egenskap. Denna implementation kontrollerar bara om tidskostnaden från det att monitorn startades till nu är större än den användarspecificerade gränsen"
type: docs
url: /sv/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SystemTimeInterruptMonitor
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // Starta övervakning med en 5-sekunders tidsgräns
            monitor.StartMonitor(5000);

            // Visa initialt värde för IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Simulera en långvarig operation
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // Kontrollera om avbrott begärdes
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // Visa slutligt värde för IsInterruptionRequested
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Spara resultatet
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### Se även

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


