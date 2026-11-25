---
title: "InterruptMonitor.IsInterruptionRequested"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà InterruptMonitor. Contrassegna il monitor come richiedente interruzione"
type: docs
url: /it/net/aspose.cells/interruptmonitor/isinterruptionrequested/
---
## InterruptMonitor.IsInterruptionRequested property

Segna il monitor come richiedente l'interruzione

```csharp
public override bool IsInterruptionRequested { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class InterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Crea una nuova cartella di lavoro e accedi al suo primo foglio di lavoro
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un monitor di interruzione e assegnalo alla cartella di lavoro
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Mostra lo stato iniziale di IsInterruptionRequested
            Console.WriteLine("Initial IsInterruptionRequested value: " + monitor.IsInterruptionRequested);

            // Simula un'operazione di elaborazione dati a lunga durata
            Console.WriteLine("Starting data processing...");
            for (int rowIdx = 0; rowIdx < 10000; rowIdx++)
            {
                // Richiedi l'interruzione dopo l'elaborazione di 500 righe
                if (rowIdx == 500)
                {
                    monitor.Interrupt();
                    Console.WriteLine("Interrupt requested. IsInterruptionRequested: " + monitor.IsInterruptionRequested);
                }

                // Verifica la richiesta di interruzione
                if (monitor.IsInterruptionRequested)
                {
                    Console.WriteLine($"Processing interrupted at row {rowIdx}");
                    break;
                }

                // Simula l'elaborazione dei dati
                worksheet.Cells[rowIdx, 0].Value = $"Row {rowIdx} data";
            }

            // Salva la cartella di lavoro modificata
            workbook.Save("InterruptionDemoOutput.xlsx");
            Console.WriteLine("File saved with partial data due to interruption.");
        }
    }
}
```

### Vedi anche

* class [InterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


