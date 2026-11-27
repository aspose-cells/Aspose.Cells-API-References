---
title: "InterruptMonitor.IsInterruptionRequested"
second_title: "Aspose.Cells för .NET API‑referens"
description: "InterruptMonitor egenskap. Markera monitorn som begär avbrott"
type: docs
url: /sv/net/aspose.cells/interruptmonitor/isinterruptionrequested/
---
## InterruptMonitor.IsInterruptionRequested property

Markera övervakaren som begär avbrott

```csharp
public override bool IsInterruptionRequested { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok och öppna dess första kalkylblad
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en avbrottsmonitor och tilldela den till arbetsboken
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Visa initialt tillstånd för IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);

            // Simulera en långvarig databehandlingsoperation
            Console.WriteLine("Starting data processing...");
            for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
            {
                // Begär avbrott efter att ha bearbetat 500 rader
                if (rowIdx == 500)
                {
                    monitor.Interrupt();
                    Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
                }

                // Kontrollera avbrottsbegäran
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine($"Processing interrupted at row {rowIdx}");
                    break;
                }

                // Simulera databehandling
                worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
            }

            // Spara den modifierade arbetsboken
            workbook.Save("InterruptionDemoOutput.xlsx");
            Console.WriteLine("File saved with partial data due to interruption.");
        }
    }
}
```

### Se även

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


