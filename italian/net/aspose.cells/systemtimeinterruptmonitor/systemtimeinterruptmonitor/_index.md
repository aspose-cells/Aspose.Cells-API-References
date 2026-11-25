---
title: "SystemTimeInterruptMonitor.SystemTimeInterruptMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Costruttore SystemTimeInterruptMonitor. Costruisce un monitor di interruzione"
type: docs
url: /it/net/aspose.cells/systemtimeinterruptmonitor/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor constructor

Costruisce un monitor di interruzione.

```csharp
public SystemTimeInterruptMonitor(bool terminateWithoutException)
```

| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| terminateWithoutException | Boolean | [`TerminateWithoutException`](../../abstractinterruptmonitor/terminatewithoutexception/) |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class SystemTimeInterruptMonitorMethodCtorWithBooleanDemo
    {
        public static void Run()
        {
            // Crea un'istanza con terminateWithoutException impostato a false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Configura le opzioni di caricamento con il monitor
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Avvia il monitoraggio con limite di tempo di 1 secondo
            monitor.StartMonitor(1000);

            try
            {
                // Tentativo di caricare una cartella di lavoro
                Workbook wb = new Workbook("sample.xlsx", lopts);

                // Reimposta il monitor per l'operazione di salvataggio con limite di 1,5 secondi
                monitor.StartMonitor(1500);
                wb.Save("output.xlsx");
            }
            catch (Exception ex)
            {
                Console.WriteLine("Operation interrupted: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [SystemTimeInterruptMonitor](../)
* namespace [Aspose.Cells](../../../aspose.cells/)
* assembly [Aspose.Cells](../../../)


