---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells för .NET API‑referens"
description: "SystemTimeInterruptMonitor-egenskap. Se TerminateWithoutException. Denna egenskap specificeras av användaren när denna övervakningsinstans konstrueras."
type: docs
url: /sv/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

Se [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). Denna egenskap specificeras av användaren när denna övervakningsinstans konstrueras.

```csharp
public override bool TerminateWithoutException { get; }
```

### Exempel

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av SystemTimeInterruptMonitor med initialt värde för TerminateWithoutException
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Visa det aktuella värdet för egenskapen TerminateWithoutException
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Starta övervakning med en tidsgräns på 1000 ms
            monitor.StartMonitor(1000);

            // Demonstrera effekten av TerminateWithoutException genom att försöka en lång operation
            try
            {
                // Simulera en lång operation som kan överskrida tidsgränsen
                for (int i = 0; i < 100000; i++)
                {
                    worksheet.Cells[i, 0].Value = i;
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Operation interrupted by monitor");
                        break;
                    }
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception caught: " + ex.Message);
            }

            // Skapa en annan övervakare med TerminateWithoutException satt till true
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // Spara arbetsboken
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


