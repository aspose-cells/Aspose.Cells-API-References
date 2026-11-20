---
title: "LightCellsDataHandler"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta il gestore dei dati delle celle per la lettura di file di foglio di calcolo di grandi dimensioni in modalità leggera."
type: docs
url: /it/java/com.aspose.cells/lightcellsdatahandler/
---
```
public interface LightCellsDataHandler
```

Rappresenta il gestore dei dati delle celle per la lettura di file di foglio di calcolo di grandi dimensioni in modalità leggera.

**Remarks**

Durante la lettura di una cartella di lavoro in questa modalità, [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) verrà verificato durante la lettura di ogni foglio di lavoro nella cartella. Per un foglio, se [startSheet(Worksheet)](../../com.aspose.cells/lightcellsdatahandler\#startSheet-Worksheet-) restituisce true, tutti i dati e le proprietà delle righe/celle di questo foglio saranno controllati e elaborati dall'implementazione di questa interfaccia. Per ogni riga, verrà chiamato [startRow(int)](../../com.aspose.cells/lightcellsdatahandler\#startRow-int-) per verificare se deve essere elaborata. Se una riga deve essere elaborata, le proprietà di questa riga verranno lette per prime e l'utente potrà accedere alle sue proprietà tramite [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-). Se anche le celle della riga devono essere elaborate, allora [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-) dovrebbe restituire true e quindi [startCell(int)](../../com.aspose.cells/lightcellsdatahandler\#startCell-int-) verrà chiamato per ogni cella esistente in questa riga per verificare se una cella deve essere elaborata. Se una cella deve essere elaborata, allora [processCell(Cell)](../../com.aspose.cells/lightcellsdatahandler\#processCell-Cell-) verrà chiamato per elaborare la cella dall'implementazione di questa interfaccia.

Si prega di notare che l'utente dovrebbe operare solo sui valori e sulle proprietà dell'oggetto Row/Cell corrente fornito dal metodo corrispondente. Poiché i dati delle celle vengono letti dal file modello in modalità streaming, la maggior parte degli altri oggetti potrebbe essere ripristinata/aggiornata in seguito dopo che i dati delle celle sono stati caricati. Pertanto, quando l'utente opera su altri oggetti in questa implementazione, tali operazioni potrebbero non influire sugli oggetti esistenti nella cartella di lavoro. Ancora peggio, tali operazioni potrebbero causare dati incoerenti nella cartella di lavoro e quindi generare problemi o eccezioni inattese in seguito. Perciò, per tutti gli altri oggetti come forme, larghezza delle colonne e stili, formattazioni condizionali, ...ecc., si prega di non operarli in nessun metodo di questa implementazione. Invece, gestiteli dopo che la cartella di lavoro è stata costruita.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [processCell(Cell cell)](#processCell-com.aspose.cells.Cell-) | Inizia l'elaborazione di una cella. |
| [processRow(Row row)](#processRow-com.aspose.cells.Row-) | Inizia l'elaborazione di una riga. |
| [startCell(int columnIndex)](#startCell-int-) | Prepara l'elaborazione di una cella. |
| [startRow(int rowIndex)](#startRow-int-) | Prepara l'elaborazione di una riga. |
| [startSheet(Worksheet sheet)](#startSheet-com.aspose.cells.Worksheet-) | Inizia l'elaborazione di un foglio di lavoro. |
### processCell(Cell cell) {#processCell-com.aspose.cells.Cell-}
```
public abstract boolean processCell(Cell cell)
```


Inizia l'elaborazione di una cella.

**Remarks**

Verrà chiamato dopo che i dati di una cella sono stati letti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cell | [Cell](../../com.aspose.cells/cell) | Oggetto Cell attualmente in elaborazione |

**Returns:**
boolean - indica se questa cella deve essere mantenuta nel modello di celle del foglio corrente. In genere dovrebbe essere false in modo che tutte le celle non vengano mantenute in memoria dopo essere state elaborate, risparmiando così memoria. Per alcuni scopi speciali, ad esempio se l'utente deve accedere a alcune celle in seguito dopo che l'intera cartella di lavoro è stata elaborata, l'utente può far restituire true a questo metodo per mantenere quelle celle speciali nel modello Cells e accedervi successivamente tramite API come Cells[row, column]. Tuttavia, mantenere i dati delle celle nel modello Cells richiederà più memoria e, se tutte le celle vengono mantenute, la lettura del file modello in modalità LightCells diventerà identica alla lettura in modalità normale.
### processRow(Row row) {#processRow-com.aspose.cells.Row-}
```
public abstract boolean processRow(Row row)
```


Inizia l'elaborazione di una riga.

**Remarks**

Verrà chiamato dopo che le proprietà della riga, come altezza, stile, ...ecc., sono state lette. Tuttavia, le celle di questa riga non sono ancora state lette.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| row | [Row](../../com.aspose.cells/row) | Oggetto Row attualmente in elaborazione. |

**Returns:**
boolean - indica se le celle di questa riga devono essere elaborate. false per ignorare tutte le celle di questa riga.
### startCell(int columnIndex) {#startCell-int-}
```
public abstract boolean startCell(int columnIndex)
```


Prepara l'elaborazione di una cella.

**Remarks**

Verrà chiamato quando si raggiunge una cella esistente nella riga corrente. La riga corrente è la riga dell'ultima chiamata di [processRow(Row)](../../com.aspose.cells/lightcellsdatahandler\#processRow-Row-).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | indice della colonna della cella da elaborare |

**Returns:**
boolean - indica se questa cella deve essere elaborata. false per ignorare la cella e controllare la successiva fino a raggiungere la fine dei dati delle celle della riga corrente
### startRow(int rowIndex) {#startRow-int-}
```
public abstract boolean startRow(int rowIndex)
```


Prepara l'elaborazione di una riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | l'indice della prossima riga da elaborare |

**Returns:**
boolean - indica se questa riga (proprietà o dati delle celle) deve essere elaborata. false per ignorare questa riga e le sue celle e controllare la riga successiva.
### startSheet(Worksheet sheet) {#startSheet-com.aspose.cells.Worksheet-}
```
public abstract boolean startSheet(Worksheet sheet)
```


Inizia l'elaborazione di un foglio di lavoro.

**Remarks**

Verrà chiamato prima di leggere i dati delle celle di un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | il foglio di lavoro da cui leggere i dati delle celle. |

**Returns:**
boolean - indica se i dati delle celle di questo foglio devono essere elaborati. false per ignorare questo foglio.
