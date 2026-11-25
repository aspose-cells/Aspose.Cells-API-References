---
title: "InterruptMonitor.Interrupt"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Metodo InterruptMonitor. Interrompe l'operatore corrente"
type: docs
url: /it/net/aspose.cells/interruptmonitor/interrupt/
---
## InterruptMonitor.Interrupt method

Interrompi l'operatore corrente.

```csharp
public void Interrupt()
```

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class InterruptMonitorMethodInterruptDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati al worksheet
            Worksheet worksheet = workbook.Worksheets[0];
            for (int i = 0; i < 10000; i++)
            {
                worksheet.Cells[i, 0].Value = "Data " + i;
            }

            // Crea e imposta il monitor di interruzione
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            try
            {
                Console.WriteLine("Starting long operation...");
                
                // Simula un'operazione lunga in un altro thread
                System.Threading.ThreadPool.QueueUserWorkItem(_ => 
                {
                    System.Threading.Thread.Sleep(1000); // Wait 1 second
                    Console.WriteLine("Interrupting operation...");
                    monitor.Interrupt(); // Call interrupt
                });

                // Esegui un'operazione lunga (salva)
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

### Vedi anche

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


