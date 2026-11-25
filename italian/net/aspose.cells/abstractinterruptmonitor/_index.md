---
title: "Classe AbstractInterruptMonitor"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Classe Aspose.Cells.AbstractInterruptMonitor. Monitor per le richieste di interruzione in tutte le operazioni che richiedono tempo"
type: docs
url: /it/net/aspose.cells/abstractinterruptmonitor/
---
## AbstractInterruptMonitor class

Monitor per le richieste di interruzione in tutte le operazioni che richiedono molto tempo.

```csharp
public abstract class AbstractInterruptMonitor
```

## Proprietà

| Nome | Descrizione |
| --- | --- |
| abstract [IsInterruptionRequested](../../aspose.cells/abstractinterruptmonitor/isinterruptionrequested/) { get; } | Indica se è richiesta un'interruzione per l'operazione corrente. Se true, l'operazione corrente verrà interrotta. L'implementazione dovrebbe eseguire qui un controllo rapido ed efficiente, altrimenti potrebbe diventare un altro collo di bottiglia per la procedura. |
| virtual [TerminateWithoutException](../../aspose.cells/abstractinterruptmonitor/terminatewithoutexception/) { get; } | Quando la procedura è interrotta, se terminare la procedura silenziosamente o lanciare un'Exception. Il valore predefinito è false, cioè, quando [`IsInterruptionRequested`](./isinterruptionrequested/) è true, verrà lanciata una [`CellsException`](../cellsexception/) con codice Interrupted. |

### Esempi

```csharp
using Aspose.Cells;
using System;
using System.Reflection.Metadata.Ecma335;

namespace AsposeCellsExamples
{
    // Implementazione personalizzata di AbstractInterruptMonitor
    public class CustomInterruptMonitor : AbstractInterruptMonitor
    {
        //il file di risultato è corretto
        public override bool IsInterruptionRequested
        {
            get
            {
                Console.WriteLine("Get the return value of whether to interrupt the program===");
                // Logica per determinare se è richiesta l'interruzione
                return false; // Change this based on your logic
            }
        }

        public override bool TerminateWithoutException
        {
            get => false; // Change this based on your logic
        }

        //// il file di risultato si blocca
        //public override bool IsInterruptionRequested
        //{
        //    get
        //    {
        //        Console.WriteLine(\"Ottieni il valore di ritorno per sapere se interrompere il programma===\");
        //        // Logica per determinare se è richiesta l'interruzione
        //        //return false; // Modifica questo in base alla tua logica
        //        return true;
        //    }
        //}

        //public override bool TerminateWithoutException
        //{
        //    get => true; // Modifica questo in base alla tua logica
        //}
    }

    public class InterruptMonitorDemo
    {
        public static void RunDemo()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet sheet = workbook.Worksheets[0];

            // Aggiungi alcuni dati di esempio
            sheet.Cells["A1"].PutValue(10);
            sheet.Cells["A2"].PutValue(20);
            sheet.Cells["A3"].Formula = "=A1+A2";

            // Crea un'istanza di CustomInterruptMonitor
            CustomInterruptMonitor monitor = new CustomInterruptMonitor();

            // Imposta le opzioni di caricamento con il monitor di interruzione personalizzato
            LoadOptions loadOptions = new LoadOptions
            {
                InterruptMonitor = monitor
            };

            // Carica la cartella di lavoro con le opzioni specificate
            workbook = new Workbook("Sample.xlsx", loadOptions);

            // Esegui i calcoli
            workbook.CalculateFormula();

            // Salva la cartella di lavoro
            workbook.Save("InterruptMonitorDemo.xlsx");
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


