---
title: "InterruptMonitor.Interrupt"
second_title: "Aspose.Cells für .NET API‑Referenz"
description: "InterruptMonitor-Methode. Unterbrechen Sie den aktuellen Operator"
type: docs
url: /de/net/aspose.cells/interruptmonitor/interrupt/
---
## InterruptMonitor.Interrupt method

Den aktuellen Vorgang unterbrechen.

```csharp
public void Interrupt()
```

### Beispiele

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InterruptMonitorMethodInterruptDemo
    {
        public static void Run()
        {
            // Erstelle ein neues Arbeitsbuch
            Workbook workbook = new Workbook();
            
            // Füge dem Arbeitsblatt einige Daten hinzu
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 10000; i++)
            {
                worksheet.Cells[i, 0].Value = "Data " + i;
            }

            // Erstellen und setzen Sie den Interrupt-Monitor
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            try
            {
                Console.WriteLine("Starting long operation...");
                
                // Simulieren Sie einen langen Vorgang in einem anderen Thread
                System.Threading.ThreadPool.QueueUserWorkItem(_ => 
                {
                    System.Threading.Thread.Sleep(1000); // Wait 1 second
                    Console.WriteLine("Interrupting operation...");
                    monitor.Interrupt(); // Call interrupt
                });

                // Führen Sie einen langen Vorgang (Speichern) aus
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

### Siehe auch

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


