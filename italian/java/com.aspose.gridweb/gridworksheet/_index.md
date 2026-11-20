---
title: "GridWorksheet"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula l'oggetto che rappresenta un singolo foglio di lavoro."
type: docs
url: /it/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

Incapsula l'oggetto che rappresenta un singolo foglio di lavoro.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | Imposta l'intervallo a cui si applica l'AutoFiltro specificato. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | Aggiungi filtro personalizzato per la riga specificata. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Adatta automaticamente la larghezza della colonna. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | Adatta automaticamente la larghezza della colonna. |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | Adatta automaticamente l'altezza della riga. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | Adatta automaticamente l'altezza della riga. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | Adatta automaticamente l'altezza della riga in un intervallo rettangolare. |
| [autoFitRows()](#autoFitRows--) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | Adatta automaticamente tutte le righe in questo foglio di lavoro. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | Adatta automaticamente l'altezza della riga in un intervallo. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | Calcola una formula. |
| [clearComments()](#clearComments--) | Cancella tutti i commenti nel foglio di calcolo del designer. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | Copia contenuti e formati da un altro foglio di lavoro. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | Crea subtotale nel foglio. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Crea subtotale nel foglio. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | Imposta il filtro per la colonna. Nota: dobbiamo chiamare AddAutoFilter prima di chiamare filterString. La stringa dei criteri del filtro. Nota: usiamo la virgola -> \",\" come carattere di separazione, quindi il valore della cella che vuoi filtrare non deve contenere virgole. filterString(10,\"123,456\") significa che la colonna 10 deve contenere 123 o 456, filterString(10,\"123\") significa che la colonna 10 deve contenere 123. L'indice della colonna è separato da virgole, es. 123,456,789 o abc |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [getActiveCell()](#getActiveCell--) | Ottiene la cella attiva nel foglio di lavoro. |
| [getBackgroundImage()](#getBackgroundImage--) | Ottiene l'immagine di sfondo del foglio di lavoro. |
| [getCells()](#getCells--) | Ottiene la collezione di [GridCell](../../com.aspose.gridweb/gridcell). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | Rappresenta il nome codice del foglio di lavoro. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | Ottiene la didascalia della colonna. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | Ottiene il testo del tooltip dell'intestazione della colonna. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | Ottiene se una colonna è di sola lettura. |
| [getComments()](#getComments--) | Ottiene la collezione di [GridComment](../../com.aspose.gridweb/gridcomment). |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. |
| [getDisplayZeros()](#getDisplayZeros--) | Vero se i valori zero sono visualizzati. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | Rappresenta l'indice della prima colonna visibile. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | Rappresenta l'indice della prima riga visibile. |
| [getFreezedPanes()](#getFreezedPanes--) | Ottiene i riquadri di blocco. |
| [getGridActiveCell()](#getGridActiveCell--) | Ottiene la cella attiva nel foglio di lavoro. |
| [getHyperlinks()](#getHyperlinks--) | Ottiene la collezione di [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection). |
| [getIndex()](#getIndex--) | Ottiene l'indice del foglio nella raccolta di fogli di lavoro. |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | Ottiene se la cella è di sola lettura. Questo è un attributo esteso di GridWeb, non verrà mantenuto nel file Excel reale. |
| [getName()](#getName--) | Ottiene il nome del foglio di lavoro. |
| [getOutlineShown()](#getOutlineShown--) | Indica se mostrare la struttura. |
| [getPictures()](#getPictures--) | Ottiene una collezione di [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--). |
| [getPivotTables()](#getPivotTables--) | Ottiene le tabelle pivot nel foglio di lavoro. |
| [getRowCaption(int row)](#getRowCaption-int-) | Ottiene la didascalia della riga. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | Ottiene il testo del tooltip dell'intestazione della riga. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | Ottiene se una riga è di sola lettura. |
| [getSelected()](#getSelected--) | Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta. |
| [getShapes()](#getShapes--) | Ottiene una collezione di [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--). |
| [getStandardHeight()](#getStandardHeight--) | Ottiene l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | Ottiene l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [getTabColor()](#getTabColor--) | Rappresenta il colore della scheda del foglio di lavoro. |
| [getUniqueID()](#getUniqueID--) | Ottiene l'UniqueID nel Control |
| [getValidations()](#getValidations--) | Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro. |
| [getVisible()](#getVisible--) | Indica se il nome di questo foglio è mostrato nelle schede dei fogli del control. |
| [getWorkbook()](#getWorkbook--) | Ottiene l'oggetto [GridWorkbook](../../com.aspose.gridweb/gridworkbook) della collezione di fogli di lavoro. |
| [getZoom()](#getZoom--) | Rappresenta il fattore di scala in percentuale. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Raggruppa le righe. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | Ottiene un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true. |
| [isProtected()](#isProtected--) | Indica se il foglio di lavoro è protetto. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | Indica se la riga di riepilogo sarà posizionata sotto le righe di dettaglio nella struttura. |
| [moveTo(int index)](#moveTo-int-) | Sposta il foglio in un'altra posizione nel foglio di calcolo. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | Aggiorna gli auto filtri per nascondere o mostrare le righe. |
| [removeAutoFilter()](#removeAutoFilter--) | Rimuove il filtro automatico del foglio di lavoro. |
| [removeSubtotal()](#removeSubtotal--) | Rimuove il subtotale creato dal metodo CreateSubtotal nel foglio. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | L'offset intero del campo su cui si desidera applicare, basato sulla prima colonna di filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0). |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | Imposta la cella attiva nel foglio di lavoro. |
| [setAllCellsEditable()](#setAllCellsEditable--) | Rende tutte le celle modificabili. Questo è un attributo esteso |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Rende tutte le celle di sola lettura. Questo è un attributo esteso; nota che questo attributo non può essere mantenuto nella cella reale, se vuoi mantenere la protezione usa setProtect |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | Imposta l'immagine di sfondo del foglio di lavoro. |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | Imposta la didascalia per la colonna. Si prega di notare che questo è un attributo di estensione e non può essere mantenuto nel file Excel. |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | Imposta il testo del tooltip dell'intestazione di colonna. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | Imposta una colonna come sola lettura così l'utente non può eliminarla dal lato client. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | Vero se i valori zero sono visualizzati. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Rende modificabile un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendi tutte le celle di sola lettura chiamando il metodo SetAllCellsReadonly. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | Rappresenta l'indice della prima colonna visibile. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | Rappresenta l'indice della prima riga visibile. |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | Imposta la cella attiva nel foglio di lavoro. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | Imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true. |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | Imposta se la cella è di sola lettura. Questo è un attributo esteso di GridWeb, non verrà mantenuto nel file Excel reale. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome del foglio di lavoro. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | Indica se mostrare la struttura. |
| [setProtect()](#setProtect--) | Protegge il foglio di lavoro. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Rende un intervallo di celle di sola lettura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Prima rendi tutte le celle modificabili chiamando il metodo SetAllCellsEditable. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | Imposta la didascalia per la riga. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | Imposta il testo del tooltip dell'intestazione di riga. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | Imposta una riga come sola lettura così l'utente non può eliminarla dal lato client. |
| [setSelected(boolean value)](#setSelected-boolean-) | Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel. |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | Indica se la riga di riepilogo sarà posizionata sotto le righe di dettaglio nella struttura. |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | Rappresenta il colore della scheda del foglio di lavoro. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica se il nome di questo foglio è mostrato nelle schede dei fogli del control. |
| [setZoom(int value)](#setZoom-int-) | Rappresenta il fattore di scala in percentuale. |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | Sblocca i riquadri nel foglio di lavoro. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | Separa le righe. |
| [unProtect()](#unProtect--) | Rimuove la protezione del foglio di lavoro. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


Imposta l'intervallo a cui si applica l'AutoFiltro specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| startColumn | int | Indice della colonna di inizio. |
| endColumn | int | Indice della colonna finale. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


Aggiungi filtro personalizzato per la riga specificata.

**Remarks**

La stringa dei criteri di filtro. Nota che usiamo , e ; come caratteri di separazione, quindi il valore della cella non deve contenere questi caratteri di separazione. Di seguito sono riportati esempi di stringhe di criteri //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int |  |
| criterio | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


Adatta automaticamente la larghezza della colonna.

**Remarks**

AutoFitColumn è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


Adatta automaticamente la larghezza della colonna.

**Remarks**

Questo metodo adatta automaticamente una riga in base al contenuto di un intervallo di celle nella riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | Indice di colonna. |
| firstRow | int | Indice della prima riga. |
| lastRow | int | Indice dell'ultima riga. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


Adatta automaticamente l'altezza della riga.

**Remarks**

AutoFitRow è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


Adatta automaticamente l'altezza della riga.

**Remarks**

Questo metodo adatta automaticamente una riga in base al contenuto di un intervallo di celle nella riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | Indice di riga. |
| firstColumn | int | Indice della prima colonna. |
| lastColumn | int | Indice dell'ultima colonna. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


Adatta automaticamente l'altezza della riga in un intervallo rettangolare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| endRow | int | Indice della riga finale. |
| startColumn | int | Indice della colonna di inizio. |
| endColumn | int | Indice della colonna finale. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


Adatta automaticamente tutte le righe in questo foglio di lavoro.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


Adatta automaticamente tutte le righe in questo foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| onlyAuto | boolean | True, ridimensiona automaticamente l'altezza della riga solo quando l'altezza della riga non è personalizzata. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


Adatta automaticamente l'altezza della riga in un intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| endRow | int | Indice della riga finale. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


Calcola una formula.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object -
### clearComments() {#clearComments--}
```
public void clearComments()
```


Cancella tutti i commenti nel foglio di calcolo del designer.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


Copia contenuti e formati da un altro foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Foglio di lavoro di origine. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


Crea subtotale nel foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnNameRowIndex | int | L'indice di riga della riga del nome colonna. |
| dataRows | int | Il numero delle righe di dati. |
| groupByColumnIndex | int | L'indice della colonna da raggruppare. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Il tipo di funzione di subtotale. |
| subtotalColumnIndexList | int[] | Gli indici delle colonne da includere nel subtotale. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


Crea subtotale nel foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnNameRowIndex | int | L'indice di riga della riga del nome colonna. |
| dataRows | int | Il numero delle righe di dati. |
| groupByColumnIndex | int | L'indice della colonna da raggruppare. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). Il tipo di funzione di subtotale. |
| subtotalColumnIndexList | int[] | Gli indici delle colonne da includere nel subtotale. |
| functionLabel | java.lang.String | L'etichetta della funzione di subtotale. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Lo stile della riga del totale generale. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | Lo stile della riga del subtotale. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). Il tipo numerico delle celle risultato del subtotale. |
| customString | java.lang.String | La stringa di formato personalizzata delle celle risultato del subtotale. Può essere null. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


Imposta il filtro per la colonna. Nota: dobbiamo chiamare AddAutoFilter prima di chiamare filterString. La stringa dei criteri del filtro. Nota: usiamo la virgola -> \",\" come carattere di separazione, quindi il valore della cella che vuoi filtrare non deve contenere virgole. filterString(10,\"123,456\") significa che la colonna 10 deve contenere 123 o 456, filterString(10,\"123\") significa che la colonna 10 deve contenere 123. L'indice della colonna è separato da virgole, es. 123,456,789 o abc

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int |  |
| criteri | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


Blocca i riquadri nella cella specificata nel foglio di lavoro.

**Remarks**

L'indice di riga e l'indice di colonna non possono entrambi essere zero. Anche il numero di righe e il numero di colonne non possono entrambi essere zero.

I primi due parametri specificano la posizione congelata e gli ultimi due parametri specificano l'area congelata nel pannello in alto a sinistra.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| colonna | int | Indice di colonna. |
| freezedRows | int | Numero di righe visibili nel pannello superiore, non superiore all'indice di riga. |
| freezedColumns | int | Numero di colonne visibili nel pannello sinistro, non superiore all'indice di colonna. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


Blocca i riquadri nella cella specificata nel foglio di lavoro.

**Remarks**

L'indice di riga e l'indice di colonna non possono entrambi essere zero. Anche il numero di righe e il numero di colonne non possono entrambi essere zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| cellName | java.lang.String | Nome della cella. |
| freezedRows | int | Numero di righe visibili nel pannello superiore, non superiore all'indice di riga. |
| freezedColumns | int | Numero di colonne visibili nel pannello sinistro, non superiore all'indice di colonna. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


Ottiene la cella attiva nel foglio di lavoro.

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


Ottiene l'immagine di sfondo del foglio di lavoro.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


Ottiene la collezione di [GridCell](../../com.aspose.gridweb/gridcell).

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


Rappresenta il nome codice del foglio di lavoro.

**Remarks**

Non è possibile modificare il nome del codice mentre il file modello contiene VBA/macro.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


Restituisce la didascalia della colonna. Se la didascalia non è impostata, restituisce una stringa vuota.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |

**Returns:**
java.lang.String - La didascalia della colonna. Se la didascalia non è impostata, restituisce una stringa vuota.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


Ottiene il testo del tooltip dell'intestazione della colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colIndex | int | L'indice della colonna. |

**Returns:**
java.lang.String - Il testo del tooltip.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


Restituisce se una colonna è readonly. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | indice di colonna. |

**Returns:**
boolean - Se readonly restituisce true.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


Ottiene la collezione di [GridComment](../../com.aspose.gridweb/gridcomment).

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. Il valore predefinito è false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


Vero se i valori zero sono visualizzati.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


Rappresenta l'indice della prima colonna visibile.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


Rappresenta l'indice della prima riga visibile.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


Ottiene i riquadri di blocco.

**Returns:**
int[] - Restituire null significa che il foglio di lavoro non è bloccato 0:indice riga;1:colonna;2:righe bloccate;3:righe bloccate
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


Ottiene la cella attiva nel foglio di lavoro.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


Ottiene la collezione di [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection).

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ottiene l'indice del foglio nella raccolta di fogli di lavoro.

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


Ottiene se la cella è di sola lettura. Questo è un attributo esteso di GridWeb, non verrà mantenuto nel file Excel reale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int |  |
| col | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome del foglio di lavoro.

**Remarks**

La lunghezza massima del nome del foglio è 31. E non è possibile assegnare lo stesso nome (senza distinzione tra maiuscole e minuscole) a due fogli di lavoro. Ad esempio, non è possibile impostare "SheetName1" al primo foglio e impostare "SHEETNAME1" al secondo foglio.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


Indica se mostrare la struttura.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


Ottiene una collezione di [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--).

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


Ottiene le tabelle pivot nel foglio di lavoro.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


Restituisce la didascalia della riga. Se la didascalia non è impostata, restituisce una stringa vuota.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |

**Returns:**
java.lang.String - La didascalia della riga. Se la didascalia non è impostata, restituisce una stringa vuota.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


Ottiene il testo del tooltip dell'intestazione della riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | L'indice della riga. |

**Returns:**
java.lang.String - Il testo del tooltip.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


Restituisce se una riga è di sola lettura. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | indice di riga. |

**Returns:**
boolean - Se readonly restituisce true.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


Ottiene una collezione di [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--).

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


Ottiene l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


Ottiene l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel.

**Returns:**
int
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


Rappresenta il colore della scheda del foglio di lavoro.

**Remarks**

Questa funzionalità è supportata solo in ExcelXP (Excel2002) e versioni successive. Se salvi il file in formato Excel97 o Excel2000, verrà omessa.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


Ottiene l'UniqueID nel Control

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


Indica se il nome di questo foglio è mostrato nelle schede dei fogli del control.

**Returns:**
boolean
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


Ottiene l'oggetto [GridWorkbook](../../com.aspose.gridweb/gridworkbook) della collezione di fogli di lavoro.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400.

**Returns:**
int
### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


Raggruppa le righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da raggruppare. |
| lastIndex | int | L'ultimo indice di riga da raggruppare. |
| isHidden | boolean | Specifica se le righe raggruppate sono nascoste. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


Ottiene un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Indica se il foglio di lavoro è protetto.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


Indica se la riga di riepilogo sarà posizionata sotto le righe di dettaglio nella struttura.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


Sposta il foglio in un'altra posizione nel foglio di calcolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Indice del foglio di destinazione. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


Aggiorna gli auto filtri per nascondere o mostrare le righe.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


Rimuove il filtro automatico del foglio di lavoro.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


Rimuove il subtotale creato dal metodo CreateSubtotal nel foglio.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


L'offset intero del campo su cui si desidera applicare, basato sulla prima colonna di filtro (da sinistra dell'elenco; il campo più a sinistra è il campo 0).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


Imposta la cella attiva nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


Rende tutte le celle modificabili. Questo è un attributo esteso

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


Rende tutte le celle di sola lettura. Questo è un attributo esteso; nota che questo attributo non può essere mantenuto nella cella reale, se vuoi mantenere la protezione usa setProtect

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


Imposta l'immagine di sfondo del foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


Imposta la didascalia per la colonna. Si prega di notare che questo è un attributo di estensione e non può essere mantenuto nel file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colonna | int | Indice di colonna. |
| didascalia | java.lang.String | La didascalia della colonna. Passa null o una stringa vuota se vuoi annullare la didascalia. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


Imposta il testo del tooltip dell'intestazione di colonna.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| colIndex | int | L'indice della colonna. |
| tooltip | java.lang.String | Il testo del tooltip. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


Imposta una colonna come di sola lettura così l'utente non può eliminarla dal lato client. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | indice di colonna. |
| isReadonly | boolean | vero o falso. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


Indica se il foglio di lavoro specificato è visualizzato da destra a sinistra invece che da sinistra a destra. Il valore predefinito è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


Vero se i valori zero sono visualizzati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


Rende modificabile un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendi tutte le celle di sola lettura chiamando il metodo SetAllCellsReadonly. poi chiama questo metodo per specificare l'intervallo di celle da rendere modificabile

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | La riga iniziale dell'intervallo. |
| startColumn | int | La colonna iniziale dell'intervallo. |
| righe | int | Il numero delle righe. |
| colonne | int | Il numero delle colonne. |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


Rappresenta l'indice della prima colonna visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


Rappresenta l'indice della prima riga visibile.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


Imposta la cella attiva nel foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


Imposta un valore che indica se le linee della griglia sono visibili. Il valore predefinito è true.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


Imposta se la cella è di sola lettura. Questo è un attributo esteso di GridWeb, non verrà mantenuto nel file Excel reale.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int |  |
| col | int |  |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome del foglio di lavoro.

**Remarks**

La lunghezza massima del nome del foglio è 31. E non è possibile assegnare lo stesso nome (senza distinzione tra maiuscole e minuscole) a due fogli di lavoro. Ad esempio, non è possibile impostare "SheetName1" al primo foglio e impostare "SHEETNAME1" al secondo foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


Indica se mostrare la struttura.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


Protegge il foglio di lavoro.

**Remarks**

Questo metodo protegge il foglio di lavoro senza password. Può proteggere il foglio di lavoro in tutte le versioni del file Excel.

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


Rende di sola lettura un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Prima rendi tutte le celle modificabili chiamando il metodo SetAllCellsEditable. poi chiama questo metodo per specificare l'intervallo di celle da rendere di sola lettura

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | La riga iniziale dell'intervallo. |
| startColumn | int | La colonna iniziale dell'intervallo. |
| righe | int | Il numero delle righe. |
| colonne | int | Il numero delle colonne. |

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


Imposta la didascalia per la riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int | Indice di riga. |
| didascalia | java.lang.String | La didascalia della riga. Passa null o una stringa vuota se vuoi annullare la didascalia. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


Imposta il testo del tooltip dell'intestazione di riga.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | L'indice della riga. |
| tooltip | java.lang.String | Il testo del tooltip. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


Imposta una riga come di sola lettura così l'utente non può eliminarla dal lato client. questo è un metodo esteso di GridWeb specificamente, non verrà mantenuto né avrà effetto nel file Excel reale

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowIndex | int | indice di riga. |
| isReadonly | boolean | vero o falso. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


Indica se questo foglio di lavoro è selezionato quando la cartella di lavoro viene aperta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di punti.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


Imposta l'altezza predefinita della riga in questo foglio di lavoro, in unità di pixel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


Indica se la riga di riepilogo sarà posizionata sotto le righe di dettaglio nella struttura.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


Rappresenta il colore della scheda del foglio di lavoro.

**Remarks**

Questa funzionalità è supportata solo in ExcelXP (Excel2002) e versioni successive. Se salvi il file in formato Excel97 o Excel2000, verrà omessa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica se il nome di questo foglio è mostrato nelle schede dei fogli del control.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


Rappresenta il fattore di scala in percentuale. Deve essere compreso tra 10 e 400.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


Sblocca i riquadri nel foglio di lavoro.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


Separa le righe.

**Remarks**

Rimuove solo le informazioni del gruppo esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da separare. |
| lastIndex | int | L'ultimo indice di riga da separare. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


Rimuove la protezione del foglio di lavoro.

### wait() {#wait--}
```
public final void wait()
```




### wait(long arg0) {#wait-long-}
```
public final native void wait(long arg0)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

