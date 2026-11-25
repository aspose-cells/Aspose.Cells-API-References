---
title: "SystemTimeInterruptMonitor.TerminateWithoutException"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Proprietà SystemTimeInterruptMonitor. Vedi TerminateWithoutException. Questa proprietà è specificata dall'utente durante la costruzione di questa istanza del monitor."
type: docs
url: /it/net/aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/
---
## SystemTimeInterruptMonitor.TerminateWithoutException property

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

    public class SystemTimeInterruptMonitorPropertyTerminateWithoutExceptionDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di SystemTimeInterruptMonitor con il valore iniziale di TerminateWithoutException
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Mostra il valore corrente della proprietà TerminateWithoutException
            Console.WriteLine("Current TerminateWithoutException value: " + monitor.TerminateWithoutException);

            // Avvia il monitoraggio con un limite di tempo di 1000 ms
            monitor.StartMonitor(1000);

            // Dimostra l'effetto di TerminateWithoutException tentando un'operazione lunga
            try
            {
                // Simula un'operazione lunga che potrebbe superare il limite di tempo
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

            // Crea un altro monitor con TerminateWithoutException impostato su true
            SystemTimeInterruptMonitor monitorNoException = new SystemTimeInterruptMonitor(true);
            Console.WriteLine("New monitor TerminateWithoutException value: " + monitorNoException.TerminateWithoutException);

            // Salva la cartella di lavoro
            workbook.Save("PropertyTerminateWithoutExceptionDemo.xlsx");
        }
    }
}
```

### Vedi anche

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


