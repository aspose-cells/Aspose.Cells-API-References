---
title: "Interfaccia LightCellsDataHandler"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Aspose.Cells.LightCellsDataHandler interface. Rappresenta il gestore dei dati delle celle per la lettura di file di fogli di calcolo di grandi dimensioni in modalità leggera"
type: docs
url: /it/net/aspose.cells/lightcellsdatahandler/
---
## LightCellsDataHandler interface

Rappresenta il gestore dei dati delle celle per la lettura di file di foglio di calcolo di grandi dimensioni in modalità leggera.

```csharp
public interface LightCellsDataHandler
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [ProcessCell](../../aspose.cells/lightcellsdatahandler/processcell/)(Cell) | Inizia a elaborare una cella. |
| [ProcessRow](../../aspose.cells/lightcellsdatahandler/processrow/)(Row) | Inizia a elaborare una riga. |
| [StartCell](../../aspose.cells/lightcellsdatahandler/startcell/)(int) | Prepara l'elaborazione di una cella. |
| [StartRow](../../aspose.cells/lightcellsdatahandler/startrow/)(int) | Prepara l'elaborazione di una riga. |
| [StartSheet](../../aspose.cells/lightcellsdatahandler/startsheet/)(Worksheet) | Inizia a elaborare un foglio di lavoro. |

### Osservazioni

Durante la lettura di una cartella di lavoro in questa modalità, [`StartSheet`](./startsheet/) verrà verificato durante la lettura di ogni foglio di lavoro nella cartella. Per un foglio, se [`StartSheet`](./startsheet/) restituisce true, tutti i dati e le proprietà delle righe/celle di quel foglio saranno controllati ed elaborati dall'implementazione di questa interfaccia. Per ogni riga, verrà chiamato [`StartRow`](./startrow/) per verificare se deve essere elaborata. Se una riga deve essere elaborata, le sue proprietà verranno lette prima e l'utente potrà accedervi tramite [`ProcessRow`](./processrow/). Se anche le celle della riga devono essere elaborate, allora [`ProcessRow`](./processrow/) dovrebbe restituire true e successivamente verrà chiamato [`StartCell`](./startcell/) per ogni cella esistente in quella riga per verificare se una cella deve essere elaborata. Se una cella deve essere elaborata, verrà chiamato [`ProcessCell`](./processcell/) per elaborare la cella mediante l'implementazione di questa interfaccia.  Si prega di notare che l'utente dovrebbe operare solo sui valori e sulle proprietà dell'oggetto Row/Cell corrente fornito dal metodo corrispondente. Poiché i dati delle celle vengono letti dal file modello in modalità streaming, la maggior parte degli altri oggetti potrebbe essere reimpostata/aggiornata successivamente dopo il caricamento dei dati delle celle. Pertanto, quando l'utente opera su altri oggetti in questa implementazione, tali operazioni potrebbero non influire sugli oggetti presenti nella cartella di lavoro. O, peggio ancora, potrebbero causare dati incoerenti nella cartella di lavoro e generare problemi o eccezioni in seguito. Quindi, per tutti gli altri oggetti come forme, larghezza delle colonne e stili, formattazioni condizionali, ...etc., si prega di non operarli in alcun metodo di questa implementazione. Invece, gestiteli dopo che la cartella di lavoro è stata costruita.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataHandlerDemo : LightCellsDataHandler
    {
        public static void LightCellsDataHandlerExample()
        {
            // Crea una cartella di lavoro e caricala con LightCellsDataHandler
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un'istanza di LightCellsDataHandlerDemo
            LightCellsDataHandlerDemo handler = new LightCellsDataHandlerDemo();

            // Imposta il LightCellsDataHandler per la cartella di lavoro
            LoadOptions loadOptions = new LoadOptions();
            loadOptions.LightCellsDataHandler = handler;

            // Carica la cartella di lavoro con le opzioni di caricamento specificate
            workbook = new Workbook("LargeFile_original.xlsx", loadOptions);

            // Salva la cartella di lavoro per dimostrare il processo
            workbook.Save("ProcessedLargeFile.xlsx");
        }

        // Implementa il metodo StartSheet
        public bool StartSheet(Worksheet sheet)
        {
            Console.WriteLine("Starting to process sheet: " + sheet.Name);
            return true; // Continue processing
        }

        // Implementa il metodo StartRow
        public bool StartRow(int rowIndex)
        {
            Console.WriteLine("Starting to process row: " + rowIndex);
            return true; // Continue processing
        }

        // Implementa il metodo ProcessRow
        public bool ProcessRow(Row row)
        {
            Console.WriteLine("Processing row: " + row.Index);
            return true; // Continue processing
        }

        // Implementa il metodo StartCell
        public bool StartCell(int columnIndex)
        {
            Console.WriteLine("Starting to process cell in column: " + columnIndex);
            return true; // Continue processing
        }

        // Implementa il metodo ProcessCell
        public bool ProcessCell(Cell cell)
        {
            Console.WriteLine("Processing cell: " + cell.Name + " with value: " + cell.StringValue);
            return true; // Continue processing
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


