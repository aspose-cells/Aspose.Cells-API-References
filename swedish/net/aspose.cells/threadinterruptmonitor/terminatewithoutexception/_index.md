---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "Aspose.Cells för .NET API‑referens"
description: "ThreadInterruptMonitor egenskap. Se TerminateWithoutException. Denna egenskap specificeras av användaren när denna monitorinstans konstrueras."
type: docs
url: /sv/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

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

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Skapa en instans av ThreadInterruptMonitor med initialt värde för TerminateWithoutException
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // Visa det aktuella värdet av egenskapen
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Starta övervakning med en 5 sekunders gräns
            monitor.StartMonitor(5000);

            // Demonstrera bearbetning som kan avbrytas
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // Simulera lång bearbetning
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine("Processing was interrupted");
                        break;
                    }
                    worksheet.Cells[i, 0].Value = "Value " + i;
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("Exception occurred: " + ex.Message);
            }
            finally
            {
                monitor.FinishMonitor();
            }

            // Skapa en annan övervakare med TerminateWithoutException satt till true
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // Spara resultatet
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Se även

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


