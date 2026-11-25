---
title: "AbstractInterruptMonitor.IsInterruptionRequested"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà AbstractInterruptMonitor. Indica se è richiesta un'interruzione per l'operazione corrente. Se true l'operazione corrente verrà interrotta. L'implementazione dovrebbe eseguire qui un controllo rapido ed efficiente, altrimenti potrebbe diventare un altro collo di bottiglia per la procedura"
type: docs
url: /it/net/aspose.cells/abstractinterruptmonitor/isinterruptionrequested/
---
## AbstractInterruptMonitor.IsInterruptionRequested property

Indica se è richiesta un'interruzione per l'operazione corrente. Se true, l'operazione corrente verrà interrotta. L'implementazione dovrebbe eseguire qui un controllo rapido ed efficiente, altrimenti potrebbe diventare un altro collo di bottiglia per la procedura.

```csharp
public abstract bool IsInterruptionRequested { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;
    using System.Threading;
    using System.Threading.Tasks;

    public class AbstractInterruptMonitorPropertyIsInterruptionRequestedDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un monitor di interruzione e assegnalo alla cartella di lavoro
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;

            // Visualizza il valore iniziale
            Console.WriteLine("Initial IsInterruptionRequested: " + monitor.IsInterruptionRequested);

            // Avvia attività di interruzione
            Task.Run(() =>
            {
                Thread.Sleep(1000); // Wait 1 seconds
                Console.WriteLine("\nTriggering interruption...");
                monitor.Interrupt();
            });

            // Simulazione di operazione a lunga durata
            Console.WriteLine("Starting data generation...");
            try
            {
                for (int i = 0; i < 500000000; i++)
                {
                    if (monitor.IsInterruptionRequested)
                    {
                        Console.WriteLine($"\nInterrupted at row {i}");
                        break;
                    }

                    worksheet.Cells[i, 0].Value = $"Data {i}";
                    
                    // Simula il tempo di elaborazione
                    if (i % 1000 == 0) 
                        Console.Write(".");
                }
            }
            catch (Exception ex)
            {
                Console.WriteLine("\nError: " + ex.Message);
            }

            // Salva il risultato
            workbook.Save("InterruptionDemoOutput.xlsx");

            Console.WriteLine("\nWorkbook saved with partial data.");
        }
    }
}
```

### Vedi anche

* class [AbstractInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


