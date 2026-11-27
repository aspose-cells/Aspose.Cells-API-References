---
title: "InterruptMonitor.Interrupt"
second_title: "Aspose.Cells för .NET API‑referens"
description: "InterruptMonitor metod. Avbryt den aktuella operatören"
type: docs
url: /sv/net/aspose.cells/interruptmonitor/interrupt/
---
## InterruptMonitor.Interrupt method

Avbryt den aktuella operatören.

```csharp
public void Interrupt()
```

### Exempel

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InterruptMonitorMethodInterruptDemo
    {
        public static void Run()
        {
            // Skapa en ny arbetsbok
            Workbook workbook = new Workbook();
            
            // Lägg till lite data i kalkylbladet
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 10000; i++)
            {
                worksheet.Cells[i, 0].Value = "Data " + i;
            }

            // Skapa och ställ in avbrottsmonitor
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            try
            {
                Console.WriteLine("Starting long operation...");
                
                // Simulera en lång operation i en annan tråd
                System.Threading.ThreadPool.QueueUserWorkItem(_ => 
                {
                    System.Threading.Thread.Sleep(1000); // Wait 1 second
                    Console.WriteLine("Interrupting operation...");
                    monitor.Interrupt(); // Call interrupt
                });

                // Utför en lång operation (spara)
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Operation completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was interrupted successfully.");
                }
                else
                {
                    Console.WriteLine("Error: " + e.Message);
                }
            }
        }
    }
}
```

### Se även

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


