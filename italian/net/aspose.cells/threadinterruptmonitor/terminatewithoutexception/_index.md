---
title: "ThreadInterruptMonitor.TerminateWithoutException"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà ThreadInterruptMonitor. Vedi TerminateWithoutException. Questa proprietà è specificata dall'utente durante la costruzione di questa istanza del monitor"
type: docs
url: /it/net/aspose.cells/threadinterruptmonitor/terminatewithoutexception/
---
## ThreadInterruptMonitor.TerminateWithoutException property

Vedi [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/). Questa proprietà è specificata dall'utente durante la costruzione di questa istanza del monitor.

```csharp
public override bool TerminateWithoutException { get; }
```

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di ThreadInterruptMonitor con il valore iniziale di TerminateWithoutException
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);
            
            // Visualizza il valore corrente della proprietà
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Avvia il monitoraggio con un limite di 5 secondi
            monitor.StartMonitor(5000);

            // Dimostrare l'elaborazione che potrebbe essere interrotta
            try
            {
                for (int i = 0; i < 100000; i++)
                {
                    // Simulare un'elaborazione lunga
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

            // Crea un altro monitor con TerminateWithoutException impostato su true
            ThreadInterruptMonitor silentMonitor = new ThreadInterruptMonitor(true);
            Console.WriteLine("\nNew monitor TerminateWithoutException value: " + silentMonitor.TerminateWithoutException);

            // Salva il risultato
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [ThreadInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


