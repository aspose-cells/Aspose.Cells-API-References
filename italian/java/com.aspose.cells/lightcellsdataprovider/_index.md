---
title: "LightCellsDataProvider"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il provider di dati per il salvataggio di file di foglio di calcolo di grandi dimensioni in modalità leggera."
type: docs
url: /it/java/com.aspose.cells/lightcellsdataprovider/
---
```
public interface LightCellsDataProvider
```

Rappresenta il provider di dati per il salvataggio di file di foglio di calcolo di grandi dimensioni in modalità leggera.

**Remarks**

Durante il salvataggio di una cartella di lavoro in questa modalità, [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) verrà verificato durante il salvataggio di ogni foglio di lavoro nella cartella. Per un foglio, se [startSheet(int)](../../com.aspose.cells/lightcellsdataprovider\#startSheet-int-) restituisce true, tutti i dati e le proprietà da salvare per le righe/celle di questo foglio saranno forniti dall'implementazione di questa interfaccia. In primo luogo, [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--) verrà chiamato per ottenere l'indice della riga successiva da salvare. Se viene restituito un indice di riga valido (l'indice della riga deve essere in ordine crescente per le righe da salvare), allora un oggetto Row che rappresenta questa riga sarà fornito da [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-) affinché l'implementazione ne imposti le proprietà. Per una riga, [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--) verrà controllato per primo. Se viene restituito un indice di colonna valido (l'indice di colonna deve essere in ordine crescente per tutte le celle della riga corrente), allora un oggetto Cell che rappresenta questa cella sarà fornito da [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) per l'implementazione impostarne i dati e le proprietà. Dopo [startCell(Cell)](../../com.aspose.cells/lightcellsdataprovider\#startCell-Cell-) la cella verrà salvata direttamente nel file di foglio di calcolo risultante. Quindi la cella successiva verrà controllata e processata.

Si prega di notare, l'utente dovrebbe aggiornare solo i valori e le proprietà per l'oggetto Row/Cell corrente fornito dal metodo corrispondente. Poiché i dati delle celle vengono scritti nel file risultante in modalità streaming, la maggior parte degli altri oggetti potrebbe essere già stata scritta nel file risultante, o potrebbero essere stati raccolti e scritti alcuni dati globali per essi. Pertanto, quando l'utente aggiorna altri oggetti durante il salvataggio dei dati delle celle, tali operazioni potrebbero non influire sui dati salvati. O, peggio ancora, tali operazioni potrebbero causare il salvataggio di dati incoerenti nel file risultante e infine corrompere il file. Quindi, per tutti gli altri oggetti come forme, larghezza delle colonne e stili, formattazioni condizionali, ...etc., si prega di non operarli in alcun metodo di questa implementazione. Invece, gestiteli e adattateli allo stato finale prima di chiamare il metodo "Save" del Workbook.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [isGatherString()](#isGatherString--) | Verifica se il valore stringa corrente della cella deve essere raccolto in un pool globale. |
| [nextCell()](#nextCell--) | Ottiene la cella successiva da salvare. |
| [nextRow()](#nextRow--) | Ottiene la riga successiva da salvare. |
| [startCell(Cell cell)](#startCell-com.aspose.cells.Cell-) | Inizia a salvare i dati di una cella. |
| [startRow(Row row)](#startRow-com.aspose.cells.Row-) | Inizia a salvare i dati di una riga. |
| [startSheet(int sheetIndex)](#startSheet-int-) | Inizia a salvare un foglio di lavoro. |
### isGatherString() {#isGatherString--}
```
public abstract boolean isGatherString()
```


Verifica se il valore stringa corrente della cella deve essere raccolto in un pool globale.

**Remarks**

La raccolta dei valori stringa sarà vantaggiosa solo quando ci sono molte stringhe duplicate per le celle fornite da questa implementazione. In questa situazione, raccogliere le stringhe farà risparmiare molta memoria e genererà un file risultante più piccolo. Se ci sono molte stringhe per le celle fornite da LightCellsDataProvider ma poche sono uguali, la raccolta delle stringhe richiederà più memoria e tempo e non offrirà vantaggi per il file risultante.

**Returns:**
boolean - true se il valore stringa deve essere raccolto in un pool globale per il file risultante.
### nextCell() {#nextCell--}
```
public abstract int nextCell()
```


Ottiene la cella successiva da salvare.

**Remarks**

Verrà chiamato all'inizio del salvataggio di una cella.

**Returns:**
int - indice di colonna della prossima cella da salvare. -1 indica che è stata raggiunta la fine dei dati della riga corrente e non ci sono altre celle da salvare nella riga corrente.
### nextRow() {#nextRow--}
```
public abstract int nextRow()
```


Ottiene la riga successiva da salvare.

**Remarks**

Verrà chiamato all'inizio del salvataggio di una riga e dei suoi dati delle celle (prima di [startRow(Row)](../../com.aspose.cells/lightcellsdataprovider\#startRow-Row-)).

**Returns:**
int - indice della prossima riga da salvare. -1 indica che è stata raggiunta la fine dei dati del foglio corrente e non ci sono altre righe da salvare nel foglio corrente.
### startCell(Cell cell) {#startCell-com.aspose.cells.Cell-}
```
public abstract void startCell(Cell cell)
```


Inizia a salvare i dati di una cella.

**Remarks**

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Oggetto Cell per l'implementazione per riempire i dati. Il suo indice di colonna è il valore restituito dall'ultima chiamata di [nextCell()](../../com.aspose.cells/lightcellsdataprovider\#nextCell--). Se la cella è stata inizializzata nel modello interno delle celle, verrà utilizzato l'oggetto Cell esistente. Altrimenti verrà utilizzato un oggetto Cell temporaneo per l'implementazione per riempire i dati. |

### startRow(Row row) {#startRow-com.aspose.cells.Row-}
```
public abstract void startRow(Row row)
```


Inizia a salvare i dati di una riga.

**Remarks**

Verrà chiamato all'inizio del salvataggio di una riga e dei suoi dati delle celle. Se la riga corrente ha alcune proprietà personalizzate come altezza, stile, ...etc., l'implementazione dovrebbe impostare tali proprietà sull'oggetto Row fornito qui.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Oggetto Row per l'implementazione per riempire i dati. Il suo indice di riga è il valore restituito dall'ultima chiamata di [nextRow()](../../com.aspose.cells/lightcellsdataprovider\#nextRow--). Se la riga è stata inizializzata nel modello interno delle celle, verrà utilizzato l'oggetto Row esistente. Altrimenti verrà utilizzato un oggetto Row temporaneo per l'implementazione per riempire i dati. |

### startSheet(int sheetIndex) {#startSheet-int-}
```
public abstract boolean startSheet(int sheetIndex)
```


Inizia a salvare un foglio di lavoro.

**Remarks**

Verrà chiamato all'inizio del salvataggio di un foglio di lavoro durante il salvataggio di un workbook. Se il provider deve fare riferimento a *`sheetIndex`* più tardi nei metodi startRow(Row) o startCell(Cell), cioè se il processo deve sapere quale foglio di lavoro è in fase di elaborazione, l'implementazione dovrebbe conservare il valore di *`sheetIndex`* qui.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | indice del foglio corrente da salvare. |

**Returns:**
boolean - true se questo provider fornirà dati per il foglio specificato; false se il foglio specificato deve utilizzare il suo modello di dati normale (Cells).
