---
title: "WorksheetDesign"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Ereditato da WebWorksheet."
type: docs
url: /it/java/com.aspose.gridweb/worksheetdesign/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control), [com.aspose.gridweb.WebWorksheet](../../com.aspose.gridweb/webworksheet)
```
public class WorksheetDesign extends WebWorksheet
```

Ereditato da WebWorksheet. Utilizzato solo a tempo di progettazione.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [WorksheetDesign()](#WorksheetDesign--) | Costruttore predefinito. |
| [WorksheetDesign(MainWeb mw, GridWorksheet gwk)](#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | il costruttore con MainWeb e GridWorksheet |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | Adatta automaticamente la larghezza della colonna. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | Adatta automaticamente la larghezza della colonna. |
| [cancelNewBindRow()](#cancelNewBindRow--) | Annulla ed elimina la nuova riga di binding aggiunta. |
| [commitNewBindRow()](#commitNewBindRow--) | Conferma la nuova riga di binding aggiunta e la aggiunge all'origine dati. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | Copia da un altro oggetto worksheet. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | Dopo aver impostato un'origine dati per il worksheet, chiama questo metodo per generare automaticamente le colonne di binding. |
| [createNewBindRow()](#createNewBindRow--) | Crea una nuova riga di binding e la collega all'origine dati. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | Crea subtotale nel foglio. |
| [dataBind()](#dataBind--) | Collega il foglio all'origine dati. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | Elimina una riga di binding. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | Blocca i riquadri nella cella specificata nel foglio di lavoro. |
| [getBindStartColumn()](#getBindStartColumn--) | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare all'origine dati. |
| [getBindStartRow()](#getBindStartRow--) | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare all'origine dati. |
| [getBindingSource()](#getBindingSource--) | L'oggetto origine dati effettivamente in binding durante l'esecuzione. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | Restituisce il numero di righe di binding in modalità data-binding. |
| [getDataMember()](#getDataMember--) | Restituisce il DataMember dall'origine dati multivalore. |
| [getDataSource()](#getDataSource--) | Restituisce l'origine dati. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | In modalità data-binding, indica se creare le didascalie delle intestazioni di colonna di binding nel foglio. |
| [getIndex()](#getIndex--) | Ottiene l'indice di se stesso all'interno dei fogli di lavoro. |
| [getName()](#getName--) | Ottiene il nome del foglio. |
| [getUniqueID()](#getUniqueID--) | Ottiene l'UniqueID nel Control |
| [getValidations()](#getValidations--) | Ottiene la collezione delle impostazioni di convalida dei dati nel foglio di lavoro. |
| [getVisible()](#getVisible--) | Indica se il nome di questo foglio è mostrato nelle schede dei fogli del control. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | Raggruppa le righe. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | Raggruppa le righe. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | Ottiene se il foglio di lavoro è protetto. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | Rende tutte le celle modificabili. Questo è un attributo esteso |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | Rende tutte le celle di sola lettura. Questo è un attributo esteso; nota che questo attributo non può essere mantenuto nella cella reale, se vuoi mantenere la protezione usa setProtect |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare all'origine dati. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare all'origine dati. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | Restituisce il numero di righe di binding in modalità data-binding. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | Imposta il DataMember dal multi-member DataSource. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | Imposta il DataSource. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | Rende modificabile un intervallo di celle. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Rendi tutte le celle di sola lettura chiamando il metodo SetAllCellsReadonly. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | In modalità data-binding, indica se creare le didascalie delle intestazioni di colonna di binding nel foglio. |
| [setName(String value)](#setName-java.lang.String-) | Imposta il nome del foglio. |
| [setProtected(boolean value)](#setProtected-boolean-) | Imposta se il foglio di lavoro è protetto. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | Rende un intervallo di celle di sola lettura. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells Prima rendi tutte le celle modificabili chiamando il metodo SetAllCellsEditable. |
| [setVisible(boolean value)](#setVisible-boolean-) | Indica se il nome di questo foglio è mostrato nelle schede dei fogli del control. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | Sblocca i riquadri nel foglio di lavoro. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | Separa le righe. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorksheetDesign() {#WorksheetDesign--}
```
public WorksheetDesign()
```


Costruttore predefinito.

### WorksheetDesign(MainWeb mw, GridWorksheet gwk) {#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WorksheetDesign(MainWeb mw, GridWorksheet gwk)
```


il costruttore con MainWeb e GridWorksheet

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

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

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


Adatta automaticamente la larghezza della colonna. Questo metodo adatta automaticamente una colonna in base al contenuto in un intervallo di celle all'interno della colonna da startRow a endRow. AutoFitColumn è una funzione imprecisa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| columnIndex | int | indice colonna, basato su zero |
| startRow | int | indice riga di inizio, basato su zero |
| endRow | int | indice riga di fine, basato su zero |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


Annulla ed elimina la nuova riga di binding aggiunta.

**Returns:**
int - L'indice della riga. Se non esiste una nuova riga di binding creata, restituisce -1.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


Conferma la nuova riga di binding aggiunta e la aggiunge all'origine dati.

**Returns:**
int - L'indice della riga della nuova riga. Se non viene creata alcuna riga, restituisce -1.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


Copia da un altro oggetto worksheet.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | L'altro foglio. |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


Dopo aver impostato un'origine dati per il worksheet, chiama questo metodo per generare automaticamente le colonne di binding.

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


Crea una nuova riga di binding e la collega all'origine dati.

**Returns:**
int - L'indice della riga della nuova riga. Se non viene creata alcuna riga, restituisce -1.
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

### dataBind() {#dataBind--}
```
public void dataBind()
```


Collega il foglio all'origine dati.

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


Elimina una riga di binding.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rowNum | int | L'indice della riga. |

**Returns:**
int - L'indice della riga eliminata. Se non viene eliminata alcuna riga di binding, restituisce -1.
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

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare all'origine dati.

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare all'origine dati.

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


L'oggetto datasource di binding effettivo a runtime. È un oggetto DataView quando la proprietà DataSource è un oggetto DataSet, DataTable o DataView.

**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```


Restituisce il numero di righe di binding in modalità data-binding.

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


Ottiene il DataMember dal multi-member DataSource. Generalmente rappresenta un oggetto DataTable di un DataSet.

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


Ottiene il DataSource. Generalmente è un oggetto DataSet.

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


In modalità data-binding, indica se creare le didascalie delle intestazioni di colonna di binding nel foglio.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Ottiene l'indice di se stesso all'interno dei fogli di lavoro.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


Ottiene il nome del foglio.

**Returns:**
java.lang.String
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
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


Raggruppa le righe.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da raggruppare. |
| lastIndex | int | L'ultimo indice di riga da raggruppare. |

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
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


Ottiene se il foglio di lavoro è protetto. Quando un foglio di lavoro è protetto, tutte le celle non possono essere modificate eccetto la cella la cui proprietà IsLocked è false.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




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

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare all'origine dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


In modalità data-binding, BindStartRow e BindStartColumn indicano la posizione della griglia da collegare all'origine dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


Restituisce il numero di righe di binding in modalità data-binding.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


Imposta il DataMember dal multi-member DataSource. Generalmente rappresenta un oggetto DataTable di un DataSet.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


Imposta il DataSource. Generalmente è un oggetto DataSet.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

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

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


In modalità data-binding, indica se creare le didascalie delle intestazioni di colonna di binding nel foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


Imposta il nome del foglio.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


Imposta se il foglio di lavoro è protetto. Quando un foglio di lavoro è protetto, tutte le celle non possono essere modificate eccetto la cella la cui proprietà IsLocked è false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

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

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


Indica se il nome di questo foglio è mostrato nelle schede dei fogli del control.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```


Sblocca i riquadri nel foglio di lavoro.

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


Separa le righe.

**Remarks**

Rimuove solo le informazioni del gruppo esterno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| firstIndex | int | Il primo indice di riga da separare. |
| lastIndex | int | L'ultimo indice di riga da separare. |

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

