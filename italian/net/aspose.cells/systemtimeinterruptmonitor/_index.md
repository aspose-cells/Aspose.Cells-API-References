---
title: "Classe SystemTimeInterruptMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.SystemTimeInterruptMonitor. Implementazione semplice di AbstractInterruptMonitor controllando e confrontando l'ora di sistema corrente con il limite specificato dall'utente"
type: docs
url: /it/net/aspose.cells/systemtimeinterruptmonitor/
---
## SystemTimeInterruptMonitor class

Implementazione semplice di [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) controllando e confrontando l'ora di sistema corrente con il limite specificato dall'utente.

```csharp
public class SystemTimeInterruptMonitor : AbstractInterruptMonitor
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [SystemTimeInterruptMonitor](systemtimeinterruptmonitor/)(bool) | Costruisce un monitor di interruzione. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/systemtimeinterruptmonitor/isinterruptionrequested/) { get; } | Questa implementazione verifica semplicemente se il tempo impiegato (dal momento in cui si avvia questo monitor fino a ora) è superiore al limite specificato dall'utente. |
| override [TerminateWithoutException](../../aspose.cells/systemtimeinterruptmonitor/terminatewithoutexception/) { get; } | Vedi [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Questa proprietà è specificata dall'utente durante la costruzione di questa istanza di monitor. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [StartMonitor](../../aspose.cells/systemtimeinterruptmonitor/startmonitor/)(int) | Avvia il monitor con il limite di tempo specificato. Il tempo di inizio per calcolare il tempo impiegato è proprio quando questo metodo viene chiamato, quindi la procedura da monitorare dovrebbe iniziare subito dopo questa chiamata. |

### Osservazioni

Questa implementazione è solo una soluzione semplice per scenari semplici. Necessita di recuperare e controllare frequentemente l'ora di sistema, quindi potrebbe avere un impatto negativo sulle prestazioni in una certa misura.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class SystemTimeInterruptMonitorDemo
    {
        public static void SystemTimeInterruptMonitorExample()
        {
            // Crea un'istanza di SystemTimeInterruptMonitor con terminateWithoutException impostato su false
            SystemTimeInterruptMonitor monitor = new SystemTimeInterruptMonitor(false);

            // Crea LoadOptions e imposta InterruptMonitor sul monitor creato
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Avvia il monitoraggio con un limite di tempo di 1000 millisecondi (1 secondo)
            monitor.StartMonitor(1000);

            try
            {
                // Carica una cartella di lavoro con le LoadOptions specificate
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Se il tempo di caricamento del file modello supera un secondo, sarà necessario interrompere e verrà generata un'eccezione qui
                // Altrimenti, inizia a monitorare la procedura di salvataggio con un nuovo limite di tempo
                monitor.StartMonitor(1500); // time limit is 1.5 seconds

                // Salva la cartella di lavoro
                wb.Save("SystemTimeInterruptMonitorExample.xlsx");
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

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


