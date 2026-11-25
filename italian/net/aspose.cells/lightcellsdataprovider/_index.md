---
title: "Interfaccia LightCellsDataProvider"
second_title: "Riferimento API Aspose.Cells per .NET"
description: "Interfaccia Aspose.Cells.LightCellsDataProvider. Rappresenta il provider di dati per il salvataggio di file di foglio di calcolo di grandi dimensioni in modalità leggera."
type: docs
url: /it/net/aspose.cells/lightcellsdataprovider/
---
## LightCellsDataProvider interface

Rappresenta il provider di dati per il salvataggio di file di foglio di calcolo di grandi dimensioni in modalità leggera.

```csharp
public interface LightCellsDataProvider
```

## Metodi

| Nome | Descrizione |
| --- | --- |
| [IsGatherString](../../aspose.cells/lightcellsdataprovider/isgatherstring/)() | Verifica se il valore stringa corrente della cella deve essere raccolto in un pool globale. |
| [NextCell](../../aspose.cells/lightcellsdataprovider/nextcell/)() | Ottiene la prossima cella da salvare. |
| [NextRow](../../aspose.cells/lightcellsdataprovider/nextrow/)() | Ottiene la prossima riga da salvare. |
| [StartCell](../../aspose.cells/lightcellsdataprovider/startcell/)(Cell) | Inizia a salvare i dati di una cella. |
| [StartRow](../../aspose.cells/lightcellsdataprovider/startrow/)(Row) | Inizia a salvare i dati di una riga. |
| [StartSheet](../../aspose.cells/lightcellsdataprovider/startsheet/)(int) | Inizia a salvare un foglio di lavoro. |

### Osservazioni

Durante il salvataggio di una cartella di lavoro in questa modalità, [`StartSheet`](./startsheet/) verrà controllato durante il salvataggio di ogni foglio di lavoro nella cartella. Per un foglio, se [`StartSheet`](./startsheet/) restituisce true, tutti i dati e le proprietà da salvare per le righe/celle di questo foglio saranno forniti dall'implementazione di questa interfaccia. In primo luogo, verrà chiamato [`NextRow`](./nextrow/) per ottenere l'indice della riga successiva da salvare. Se viene restituito un indice di riga valido (l'indice di riga deve essere in ordine crescente per le righe da salvare), allora un oggetto Row che rappresenta questa riga sarà fornito da [`StartRow`](./startrow/) affinché l'implementazione imposti le sue proprietà. Per una riga, [`NextCell`](./nextcell/) verrà controllato per primo. Se viene restituito un indice di colonna valido (l'indice di colonna deve essere in ordine crescente per tutte le celle della riga corrente), allora un oggetto Cell che rappresenta questa cella sarà fornito da [`StartCell`](./startcell/) affinché l'implementazione imposti i suoi dati e le sue proprietà. Dopo [`StartCell`](./startcell/) la cella sarà salvata direttamente nel file di foglio di calcolo risultante. Quindi la cella successiva sarà controllata e processata. Si prega di notare che l'utente dovrebbe aggiornare solo i valori e le proprietà dell'oggetto Row/Cell corrente fornito dal metodo corrispondente. Poiché i dati delle celle vengono scritti nel file risultante in modalità streaming, la maggior parte degli altri oggetti potrebbe già essere stata scritta nel file risultante, o potrebbero essere stati raccolti e scritti alcuni dati globali per essi. Pertanto, quando l'utente aggiorna altri oggetti durante il salvataggio dei dati delle celle, tali operazioni potrebbero non influire sui dati salvati. O, peggio ancora, tali operazioni potrebbero causare il salvataggio di dati incoerenti nel file risultante e alla fine corrompere il file. Quindi, per tutti gli altri oggetti come forme, larghezza delle colonne e stili, formattazioni condizionali, ... ecc., si prega di non operarli in alcun metodo di questa implementazione. Invece, si prega di gestirli e regolarli nello stato finale prima di chiamare il metodo "Save" della cartella di lavoro.

### Esempi

```csharp
namespace AsposeCellsExamples
{
    using Aspose.Cells;
    using System;

    public class LightCellsDataProviderDemo
    {
        public static void LightCellsDataProviderExample()
        {
            // Crea un nuovo workbook
            Workbook workbook = new Workbook();
            Worksheet worksheet = workbook.Worksheets[0];

            // Crea un LightCellsDataProvider personalizzato
            CustomLightCellsDataProvider dataProvider = new CustomLightCellsDataProvider();

            // Imposta il LightCellsDataProvider per salvare la cartella di lavoro
            OoxmlSaveOptions saveOptions = new OoxmlSaveOptions(SaveFormat.Xlsx)
            {
                LightCellsDataProvider = dataProvider
            };

            // Salva la cartella di lavoro con il LightCellsDataProvider personalizzato
            workbook.Save("LightCellsDataProviderExample.xlsx", saveOptions);
        }
    }

    public class CustomLightCellsDataProvider : LightCellsDataProvider
    {
        private int currentRow = -1;
        private int currentCell = -1;

        public bool StartSheet(int sheetIndex)
        {
            // Inizia l'elaborazione del primo foglio
            return sheetIndex == 0;
        }

        public int NextRow()
        {
            // Passa alla riga successiva
            currentRow++;
            currentCell = -1;

            // Restituisce l'indice della riga corrente o -1 se non ci sono più righe
            return currentRow < 10 ? currentRow : -1;
        }

        public void StartRow(Row row)
        {
            // Inizializza la riga se necessario
        }

        public int NextCell()
        {
            // Passa alla cella successiva
            currentCell++;

            // Restituisce l'indice della cella corrente o -1 se non ci sono più celle
            return currentCell < 10 ? currentCell : -1;
        }

        public void StartCell(Cell cell)
        {
            // Imposta il valore della cella
            cell.PutValue($"R{currentRow}C{currentCell}");
        }

        public bool IsGatherString()
        {
            // Restituisce se raccogliere le stringhe in un pool globale
            return false;
        }
    }
}
```

### Vedi anche

* namespace [Aspose.Cells](../../aspose.cells/)
* assembly [Aspose.Cells](../../)


