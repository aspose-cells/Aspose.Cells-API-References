---
title: "Classe InterruptMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.InterruptMonitor. Rappresenta tutti gli operatori relativi all'interruzione"
type: docs
url: /it/net/aspose.cells/interruptmonitor/
---
## InterruptMonitor class

Rappresenta tutti gli operatori relativi all'interruzione.

```csharp
public class InterruptMonitor : AbstractInterruptMonitor
```

## Costruttori

| Nome | Descrizione |
| --- | --- |
| [InterruptMonitor](interruptmonitor/)() | Il costruttore predefinito. |

## Proprietà

| Nome | Descrizione |
| --- | --- |
| override [IsInterruptionRequested](../../aspose.cells/interruptmonitor/isinterruptionrequested/) { get; } | Segna il monitor come richiedente l'interruzione |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Quando la procedura è interrotta, se terminare la procedura silenziosamente o lanciare un'eccezione. Il valore predefinito è false, cioè, quando [`IsInterruptionRequested`](../abstractinterruptmonitor/isinterruptionrequested/) è true, verrà lanciata una [`CellsException`](../cellsexception/) con codice Interrupted. (Ereditato da [`AbstractInterruptMonitor`](../abstractinterruptmonitor/).) |

## Metodi

| Nome | Descrizione |
| --- | --- |
| [Interrupt](../../aspose.cells/interruptmonitor/interrupt/)() | Interrompi l'operatore corrente. |

### Esempi

```csharp
using System;
using Aspose.Cells;

namespace AsposeCellsExamples
{
    public class CellsClassInterruptMonitorDemo
    {
        public static void Run()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            
            // Aggiungi alcuni dati di esempio
            Worksheet worksheet = workbook.Worksheets[0];
            worksheet.Cells["A1"].PutValue("Sample Data");
            
            // Crea e assegna il monitor di interruzione
            InterruptMonitor monitor = new InterruptMonitor();
            workbook.InterruptMonitor = monitor;
            
            try
            {
                Console.WriteLine("Starting save operation...");
                
                // Simula l'interruzione dell'operazione
                monitor.Interrupt();
                
                // Prova a salvare (dovrebbe essere interrotto)
                workbook.Save("output.pdf", SaveFormat.Pdf);
                Console.WriteLine("Save completed successfully.");
            }
            catch (CellsException e)
            {
                if (e.Code == ExceptionType.Interrupted)
                {
                    Console.WriteLine("Operation was successfully interrupted.");
                }
                else
                {
                    Console.WriteLine("Error occurred: " + e.Message);
                }
            }
        }
    }
}
```

### Vedi anche

* class [AbstractInterruptMonitor](../abstractinterruptmonitor/)
* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


