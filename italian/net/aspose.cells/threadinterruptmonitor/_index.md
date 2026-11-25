---
title: "Classe ThreadInterruptMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.ThreadInterruptMonitor. Implementazione semplice di AbstractInterruptMonitor avviando un altro thread per richiedere l'interruzione dopo aver atteso il limite specificato dall'utente"
type: docs
url: /it/net/aspose.cells/threadinterruptmonitor/
---
## ThreadInterruptMonitor class

Implementazione semplice di [`AbstractInterruptMonitor`](../abstractinterruptmonitor/) avviando un altro thread per richiedere l'interruzione dopo aver atteso il limite specificato dall'utente.

```csharp
public class ThreadInterruptMonitor : AbstractInterruptMonitor
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [ThreadInterruptMonitor](threadinterruptmonitor/)(bool) | Costruisce un monitor di interruzione. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/threadinterruptmonitor/isinterruptionrequested/) { get; } | Questa implementazione verifica semplicemente se il tempo impiegato (dal momento in cui si avvia questo monitor fino a ora) è superiore al limite specificato dall'utente. |
| override [TerminateWithoutException](../../aspose.cells/threadinterruptmonitor/terminatewithoutexception/) { get; } | Vedi [`TerminateWithoutException`](../abstractinterruptmonitor/terminatewithoutexception/). Questa proprietà è specificata dall'utente durante la costruzione di questa istanza di monitor. |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [FinishMonitor](../../aspose.cells/threadinterruptmonitor/finishmonitor/)() | Conclude il monitor per una procedura. |
| [StartMonitor](../../aspose.cells/threadinterruptmonitor/startmonitor/)(int) | Avvia il monitor con il limite di tempo specificato. Il tempo di inizio per calcolare il tempo impiegato è proprio quando questo metodo viene chiamato, quindi la procedura da monitorare dovrebbe iniziare subito dopo questa chiamata. |

### Osservazioni

Un'istanza del monitor può essere usata ripetutamente, finché si monitora ogni processo in sequenza. Non dovrebbe essere usata per monitorare più procedure contemporaneamente in thread multipli.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class ThreadInterruptMonitorDemo
    {
        public static void ThreadInterruptMonitorExample()
        {
            // Crea un'istanza di ThreadInterruptMonitor con terminateWithoutException impostato su false
            ThreadInterruptMonitor monitor = new ThreadInterruptMonitor(false);

            // Crea LoadOptions e imposta InterruptMonitor sul monitor creato
            LoadOptions lopts = new LoadOptions();
            lopts.InterruptMonitor = monitor;

            // Avvia il monitor con un limite di tempo di 1000 millisecondi (1 secondo)
            monitor.StartMonitor(1000);

            try
            {
                // Carica una cartella di lavoro con le LoadOptions specificate
                Workbook wb = new Workbook("Large.xlsx", lopts);

                // Concludi il monitor per la procedura di caricamento
                monitor.FinishMonitor();

                // Avvia nuovamente il monitor con un nuovo limite di tempo di 1500 millisecondi (1,5 secondi)
                monitor.StartMonitor(1500);

                // Salva la cartella di lavoro
                wb.Save("result.xlsx");

                // Concludi il monitor per la procedura di salvataggio
                monitor.FinishMonitor();
            }
            catch (Exception ex)
            {
                Console.WriteLine("An exception occurred: " + ex.Message);
            }
        }
    }
}
```

### Vedi anche

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


