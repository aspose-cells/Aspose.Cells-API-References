---
title: "ThreadInterruptMonitor.IsInterruptionRequested"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadInterruptMonitor. Questa implementazione verifica semplicemente se il tempo trascorso dal momento in cui si avvia questo monitor fino a ora è maggiore del limite specificato dall'utente"
type: docs
url: /it/net/aspose.cells/threadinterruptmonitor/isinterruptionrequested/
---
## ThreadInterruptMonitor.IsInterruptionRequested property

Questa implementazione verifica semplicemente se il tempo impiegato (dal momento in cui si avvia questo monitor fino a ora) è superiore al limite specificato dall'utente.

```csharp
public override bool IsInterruptionRequested { get; }
```

### Esempi

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
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di ThreadInterruptMonitor
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(terminateWithoutException: false);

            // Avvia il monitoraggio con un limite di 2 secondi
            monitor.StartMonitor(2000);

            // Simula un'operazione a lungo termine
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100; i++)
            {
                // Verifica se è stata richiesta un'interruzione
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation was interrupted!");
                    break;
                }

                // Simula lavoro
                Thread.Sleep(100);
                worksheet.Cells[i, 0].Value = $"Processed row {i}";
                Console.WriteLine($"Processed row {i}");
            }

            // Termina il monitoraggio
            monitor.FinishMonitor();

            // Salva il risultato
            workbook.Save("ThreadInterruptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


