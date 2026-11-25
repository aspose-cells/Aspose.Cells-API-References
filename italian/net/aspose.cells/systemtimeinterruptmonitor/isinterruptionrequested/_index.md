---
title: "SystemTimeInterruptMonitor.IsInterruptionRequested"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SystemTimeInterruptMonitor. Questa implementazione verifica semplicemente se il costo temporale dal momento in cui si avvia questo monitor fino a ora è maggiore del limite specificato dall'utente"
type: docs
url: /it/net/aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/
---
## SystemTimeInterruptMonitor.IsInterruptionRequested property

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

    public class SystemTimeInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SystemTimeInterruptMonitor
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);
            
            // Avvia il monitoraggio con un limite di tempo di 5 secondi
            monitor.StartMonitor(5000);

            // Mostra il valore iniziale di IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Simula un'operazione a lunga durata
            Console.WriteLine("Starting long operation...");
            for (int i = 0; i < 100000; i++)
            {
                worksheet.Cells[i, 0].Value = i;
                
                // Verifica se è stata richiesta un'interruzione
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine("Operation interrupted after time limit!");
                    break;
                }
            }

            // Mostra il valore finale di IsInterruptionRequested
            Console.WriteLine("Final IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Salva il risultato
            workbook.Save("PropertyIsInterruptionRequestedDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


