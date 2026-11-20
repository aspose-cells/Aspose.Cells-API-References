---
title: "WorksheetCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Incapsula una raccolta di oggetti."
type: docs
url: /it/java/com.aspose.cells/worksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class WorksheetCollection extends CollectionBase
```

Incapsula una collezione di oggetti [Worksheet](../../com.aspose.cells/worksheet).

**Example**

```
         Workbook workbook = new Workbook();
 
         WorksheetCollection sheets = workbook.getWorksheets();
 
         //Add a worksheet
         sheets.add();
 
         //Change the name of a worksheet
         sheets.get(0).setName("First Sheet");
 
         //Set the active sheet to the second worksheet
         sheets.setActiveSheetIndex(1);
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add()](#add--) | Aggiunge un foglio di lavoro alla raccolta. |
| [add(int type)](#add-int-) | Aggiunge un foglio di lavoro alla raccolta. |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String sheetName)](#add-java.lang.String-) | Aggiunge un foglio di lavoro alla raccolta. |
| [addCopy(Worksheet[] source, String[] destSheetNames)](#addCopy-com.aspose.cells.Worksheet---java.lang.String---) | Copia un gruppo di fogli di lavoro. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente. |
| [clear()](#clear--) | Cancella tutti i fogli di lavoro. |
| [clearPivottables()](#clearPivottables--) | Rimuove le tabelle pivot dal foglio di calcolo. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [createRange(String address, int sheetIndex)](#createRange-java.lang.String-int-) | Crea un oggetto [Range](../../com.aspose.cells/range) da un indirizzo dell'intervallo. |
| [createUnionRange(String address, int sheetIndex)](#createUnionRange-java.lang.String-int-) | Crea un oggetto [Range](../../com.aspose.cells/range) da un indirizzo dell'intervallo. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene l'elemento [Worksheet](../../com.aspose.cells/worksheet) all'indice specificato. |
| [get(String sheetName)](#get-java.lang.String-) | Ottiene l'elemento [Worksheet](../../com.aspose.cells/worksheet) con il nome specificato. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto. |
| [getActiveSheetName()](#getActiveSheetName--) | Rappresenta il nome del foglio di lavoro attivo quando il foglio di calcolo è aperto. |
| [getBuiltInDocumentProperties()](#getBuiltInDocumentProperties--) | Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento integrate del foglio di calcolo. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [getCustomDocumentProperties()](#getCustomDocumentProperties--) | Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento personalizzate del foglio di calcolo. |
| [getDxfs()](#getDxfs--) | Ottiene i record di formattazione differenziale master. |
| [getExternalLinks()](#getExternalLinks--) | Rappresenta i collegamenti esterni in una cartella di lavoro. |
| [getNamedRanges()](#getNamedRanges--) | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo. |
| [getNamedRangesAndTables()](#getNamedRangesAndTables--) | Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo. |
| [getNames()](#getNames--) | Ottiene la raccolta di tutti gli oggetti Name nel foglio di calcolo. |
| [getOleSize()](#getOleSize--) | Ottiene la dimensione visualizzata quando il file Workbook è usato come oggetto OLE. |
| [getPivotCaches()](#getPivotCaches--) | Ottiene tutti i [PivotCache](../../com.aspose.cells/pivotcache). |
| [getRangeByName(String rangeName)](#getRangeByName-java.lang.String-) | Ottiene l'oggetto Range per nome predefinito. |
| [getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)](#getRangeByName-java.lang.String-int-boolean-) | Ottiene [Range](../../com.aspose.cells/range) per nome predefinito o nome della tabella |
| [getRevisionLogs()](#getRevisionLogs--) | Rappresenta i registri di revisione. |
| [getSensitivityLabels()](#getSensitivityLabels--) | Rappresenta tutte le etichette di sensibilità. |
| [getSheetByCodeName(String codeName)](#getSheetByCodeName-java.lang.String-) | Ottiene il foglio di lavoro per nome codice. |
| [getTableStyles()](#getTableStyles--) | Ottiene l'oggetto [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--). |
| [getThreadedCommentAuthors()](#getThreadedCommentAuthors--) | Ottiene l'elenco degli autori dei commenti in thread. |
| [getWebExtensionTaskPanes()](#getWebExtensionTaskPanes--) | Ottiene l'elenco dei riquadri attività. |
| [getWebExtensions()](#getWebExtensions--) | Ottiene l'elenco dei riquadri attività. |
| [getXmlMaps()](#getXmlMaps--) | Ottiene le mappe XML nella cartella di lavoro. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [insert(int index, int sheetType)](#insert-int-int-) | Inserisci un foglio di lavoro. |
| [insert(int index, int sheetType, String sheetName)](#insert-int-int-java.lang.String-) | Inserisci un foglio di lavoro. |
| [isRefreshAllConnections()](#isRefreshAllConnections--) | Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshAll()](#refreshAll--) | Aggiorna tutte le tabelle pivot e i grafici con la sorgente pivot. |
| [refreshPivotTables()](#refreshPivotTables--) | Aggiorna tutte le PivotTable nel file Excel. |
| [refreshPivotTables(PivotTableRefreshOption option)](#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-) | Aggiorna tutte le PivotTable nel file Excel. |
| [registerAddInFunction(int id, String functionName)](#registerAddInFunction-int-java.lang.String-) | Aggiunge la funzione add-in nella cartella di lavoro |
| [registerAddInFunction(String addInFile, String functionName, boolean lib)](#registerAddInFunction-java.lang.String-java.lang.String-boolean-) | Aggiunge la funzione add-in nella cartella di lavoro |
| [removeAt(int index)](#removeAt-int-) | Rimuove l'elemento a un indice specificato. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Rimuove l'elemento a un nome specificato. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto. |
| [setActiveSheetName(String value)](#setActiveSheetName-java.lang.String-) | Rappresenta il nome del foglio di lavoro attivo quando il foglio di calcolo è aperto. |
| [setOleSize(int startRow, int endRow, int startColumn, int endColumn)](#setOleSize-int-int-int-int-) | Imposta la dimensione visualizzata quando il file Cartella di lavoro è usato come oggetto OLE. |
| [setOleSize(Object value)](#setOleSize-java.lang.Object-) | Imposta la dimensione visualizzata quando il file Cartella di lavoro è usato come oggetto OLE. |
| [setRefreshAllConnections(boolean value)](#setRefreshAllConnections-boolean-) | Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel. |
| [setXmlMaps(XmlMapCollection value)](#setXmlMaps-com.aspose.cells.XmlMapCollection-) | Imposta le mappe XML nella cartella di lavoro. |
| [sortNames()](#sortNames--) | Ordina i nomi definiti. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | Scambia i due fogli. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Aggiunge un foglio di lavoro alla raccolta.

**Returns:**
int - [Foglio di lavoro](../../com.aspose.cells/worksheet) indice dell'oggetto.
### add(int type) {#add-int-}
```
public int add(int type)
```


Aggiunge un foglio di lavoro alla raccolta.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().add(SheetType.CHART);
         	Cells cells = workbook.getWorksheets().get(0).getCells();
         	cells.get("c2").putValue(5000);
         	cells.get("c3").putValue(3000);
         	cells.get("c4").putValue(4000);
         	cells.get("c5").putValue(5000);
         	cells.get("c6").putValue(6000);
         	ChartCollection charts = workbook.getWorksheets().get(1).getCharts();
         	int chartIndex = charts.add(ChartType.COLUMN, 10,10,20,20);
         	Chart chart = charts.get(chartIndex);
         	chart.getNSeries().add("Sheet1!C2:C6", true);
```

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [SheetType](../../com.aspose.cells/sheettype). Tipo di foglio di lavoro. |

**Returns:**
int - [Foglio di lavoro](../../com.aspose.cells/worksheet) indice dell'oggetto.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Aggiunge un elemento all'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | L'Object da aggiungere all'istanza di CollectionBase. |

**Returns:**
int - La posizione in cui è stato inserito il nuovo elemento.
### add(String sheetName) {#add-java.lang.String-}
```
public Worksheet add(String sheetName)
```


Aggiunge un foglio di lavoro alla raccolta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Nome del foglio di lavoro |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - [Worksheet](../../com.aspose.cells/worksheet) object.
### addCopy(Worksheet[] source, String[] destSheetNames) {#addCopy-com.aspose.cells.Worksheet---java.lang.String---}
```
public void addCopy(Worksheet[] source, String[] destSheetNames)
```


Copia un gruppo di fogli di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| source | [Worksheet\[\]](../../com.aspose.cells/worksheet) | I fogli di lavoro di origine. |
| destSheetNames | java.lang.String[] | I nomi dei fogli copiati. |

### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex | int | Indice del foglio di lavoro di origine. |

**Returns:**
int - [Foglio di lavoro](../../com.aspose.cells/worksheet) indice dell'oggetto.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Aggiunge un foglio di lavoro alla raccolta e copia i dati da un foglio di lavoro esistente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Nome del foglio di lavoro di origine. |

**Returns:**
int - [Foglio di lavoro](../../com.aspose.cells/worksheet) indice dell'oggetto.
### clear() {#clear--}
```
public void clear()
```


Cancella tutti i fogli di lavoro.

**Remarks**

Una cartella di lavoro deve contenere un foglio di lavoro.

### clearPivottables() {#clearPivottables--}
```
public void clearPivottables()
```


Rimuove le tabelle pivot dal foglio di calcolo.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Restituisce se l'istanza contiene questo oggetto

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | oggetto di test |

**Returns:**
boolean - Se l'istanza contiene questo oggetto
### createRange(String address, int sheetIndex) {#createRange-java.lang.String-int-}
```
public Range createRange(String address, int sheetIndex)
```


Crea un oggetto [Range](../../com.aspose.cells/range) da un indirizzo dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indirizzo | java.lang.String | L'indirizzo dell'intervallo. |
| sheetIndex | int | L'indice del foglio. |

**Returns:**
[Range](../../com.aspose.cells/range) - A [Range](../../com.aspose.cells/range) object
### createUnionRange(String address, int sheetIndex) {#createUnionRange-java.lang.String-int-}
```
public UnionRange createUnionRange(String address, int sheetIndex)
```


Crea un oggetto [Range](../../com.aspose.cells/range) da un indirizzo dell'intervallo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indirizzo | java.lang.String | L'indirizzo dell'intervallo. |
| sheetIndex | int | L'indice del foglio. |

**Returns:**
[UnionRange](../../com.aspose.cells/unionrange) - A [Range](../../com.aspose.cells/range) object
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
### get(int index) {#get-int-}
```
public Worksheet get(int index)
```


Ottiene l'elemento [Worksheet](../../com.aspose.cells/worksheet) all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice basato su zero dell'elemento. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public Worksheet get(String sheetName)
```


Ottiene l'elemento [Worksheet](../../com.aspose.cells/worksheet) con il nome specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetName | java.lang.String | Nome del foglio di lavoro |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto.

**Remarks**

L'indice del foglio è basato su zero.

**Returns:**
int
### getActiveSheetName() {#getActiveSheetName--}
```
public String getActiveSheetName()
```


Rappresenta il nome del foglio di lavoro attivo quando il foglio di calcolo è aperto.

**Returns:**
java.lang.String
### getBuiltInDocumentProperties() {#getBuiltInDocumentProperties--}
```
public BuiltInDocumentPropertyCollection getBuiltInDocumentProperties()
```


Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento integrate del foglio di calcolo.

**Remarks**

Non è possibile aggiungere una nuova proprietà all'elenco delle proprietà documento integrate. È possibile solo ottenere una proprietà integrata e modificarne il valore. Di seguito è l'elenco dei nomi delle proprietà integrate:

Title

Oggetto

Autore

Parole chiave

Commenti

Modello

Ultimo autore

Numero di revisione

Nome dell'applicazione

Data ultima stampa

Data di creazione

Ora ultimo salvataggio

Tempo totale di modifica

Numero di pagine

Numero di parole

Numero di caratteri

Sicurezza

Categoria

Formato

Responsabile

Azienda

Numero di byte

Numero di righe

Numero di paragrafi

Numero di diapositive

Numero di note

Numero di diapositive nascoste

Numero di clip multimediali

**Example**

```
         Workbook workbook = new Workbook();
         DocumentProperty doc = workbook.getWorksheets().getBuiltInDocumentProperties().get("Author");
         doc.setValue("John Smith");
```

**Returns:**
[BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```


Ottiene il numero di elementi contenuti nell'istanza di CollectionBase.

**Returns:**
int - Il numero di elementi contenuti nell'istanza di CollectionBase.
### getCustomDocumentProperties() {#getCustomDocumentProperties--}
```
public CustomDocumentPropertyCollection getCustomDocumentProperties()
```


Restituisce una collezione di [DocumentProperty](../../com.aspose.cells/documentproperty) che rappresenta tutte le proprietà di documento personalizzate del foglio di calcolo.

**Example**

```
         Workbook workbook = new Workbook();
         workbook.getWorksheets().getCustomDocumentProperties().add("Checked by", "Jane");
```

**Returns:**
[CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection)
### getDxfs() {#getDxfs--}
```
public DxfCollection getDxfs()
```


Ottiene i record di formattazione differenziale master.

**Returns:**
[DxfCollection](../../com.aspose.cells/dxfcollection)
### getExternalLinks() {#getExternalLinks--}
```
public ExternalLinkCollection getExternalLinks()
```


Rappresenta i collegamenti esterni in una cartella di lavoro.

**Returns:**
[ExternalLinkCollection](../../com.aspose.cells/externallinkcollection)
### getNamedRanges() {#getNamedRanges--}
```
public Range[] getNamedRanges()
```


Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo.

**Returns:**
com.aspose.cells.Range[] - Un array di oggetti Range. Se il riferimento del Nome definito è esterno o ha più intervalli, non verrà restituito alcun oggetto Range per questo Nome.

Restituisce null se l'intervallo nominato non esiste.
### getNamedRangesAndTables() {#getNamedRangesAndTables--}
```
public Range[] getNamedRangesAndTables()
```


Ottiene tutti gli intervalli denominati predefiniti nel foglio di calcolo.

**Returns:**
com.aspose.cells.Range[] - Un array di oggetti Range.

Restituisce null se l'intervallo nominato non esiste.
### getNames() {#getNames--}
```
public NameCollection getNames()
```


Ottiene la raccolta di tutti gli oggetti Name nel foglio di calcolo.

**Returns:**
[NameCollection](../../com.aspose.cells/namecollection)
### getOleSize() {#getOleSize--}
```
public Object getOleSize()
```


Ottiene la dimensione visualizzata quando il file Workbook è usato come oggetto OLE.

**Remarks**

Null indica nessuna impostazione di dimensione ole.

**Returns:**
java.lang.Object
### getPivotCaches() {#getPivotCaches--}
```
public PivotCacheCollection getPivotCaches()
```


Ottiene tutti i [PivotCache](../../com.aspose.cells/pivotcache).

**Returns:**
[PivotCacheCollection](../../com.aspose.cells/pivotcachecollection)
### getRangeByName(String rangeName) {#getRangeByName-java.lang.String-}
```
public Range getRangeByName(String rangeName)
```


Ottiene l'oggetto Range per nome predefinito.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeName | java.lang.String | Nome dell'intervallo. |

**Returns:**
[Range](../../com.aspose.cells/range) - Range object.

Restituisce null se l'intervallo nominato non esiste.
### getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable) {#getRangeByName-java.lang.String-int-boolean-}
```
public Range getRangeByName(String rangeName, int currentSheetIndex, boolean includeTable)
```


Ottiene [Range](../../com.aspose.cells/range) per nome predefinito o nome della tabella

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| rangeName | java.lang.String | Nome dell'intervallo o nome della tabella. |
| currentSheetIndex | int | Indice del foglio. -1 rappresenta globale. |
| includeTable | boolean | Indica se controllare tutte le tabelle. |

**Returns:**
[Range](../../com.aspose.cells/range) - 
### getRevisionLogs() {#getRevisionLogs--}
```
public RevisionLogCollection getRevisionLogs()
```


Rappresenta i registri di revisione.

**Returns:**
[RevisionLogCollection](../../com.aspose.cells/revisionlogcollection)
### getSensitivityLabels() {#getSensitivityLabels--}
```
public SensitivityLabelCollection getSensitivityLabels()
```


Rappresenta tutte le etichette di sensibilità.

**Returns:**
[SensitivityLabelCollection](../../com.aspose.cells/sensitivitylabelcollection)
### getSheetByCodeName(String codeName) {#getSheetByCodeName-java.lang.String-}
```
public Worksheet getSheetByCodeName(String codeName)
```


Ottiene il foglio di lavoro per nome codice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| codeName | java.lang.String | Nome codice del foglio di lavoro. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - The element with the specified code name.
### getTableStyles() {#getTableStyles--}
```
public TableStyleCollection getTableStyles()
```


Ottiene l'oggetto [getTableStyles()](../../com.aspose.cells/worksheetcollection\#getTableStyles--).

**Returns:**
[TableStyleCollection](../../com.aspose.cells/tablestylecollection)
### getThreadedCommentAuthors() {#getThreadedCommentAuthors--}
```
public ThreadedCommentAuthorCollection getThreadedCommentAuthors()
```


Ottiene l'elenco degli autori dei commenti in thread.

**Returns:**
[ThreadedCommentAuthorCollection](../../com.aspose.cells/threadedcommentauthorcollection)
### getWebExtensionTaskPanes() {#getWebExtensionTaskPanes--}
```
public WebExtensionTaskPaneCollection getWebExtensionTaskPanes()
```


Ottiene l'elenco dei riquadri attività.

**Returns:**
[WebExtensionTaskPaneCollection](../../com.aspose.cells/webextensiontaskpanecollection)
### getWebExtensions() {#getWebExtensions--}
```
public WebExtensionCollection getWebExtensions()
```


Ottiene l'elenco dei riquadri attività.

**Returns:**
[WebExtensionCollection](../../com.aspose.cells/webextensioncollection)
### getXmlMaps() {#getXmlMaps--}
```
public XmlMapCollection getXmlMaps()
```


Ottiene le mappe XML nella cartella di lavoro.

**Returns:**
[XmlMapCollection](../../com.aspose.cells/xmlmapcollection)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Determina l'indice di un elemento specifico nell'istanza di CollectionBase.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| o | java.lang.Object | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |

**Returns:**
int - L'indice del valore se trovato nella lista; altrimenti, -1.
### insert(int index, int sheetType) {#insert-int-int-}
```
public Worksheet insert(int index, int sheetType)
```


Inserisci un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice del foglio |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Il tipo di foglio. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### insert(int index, int sheetType, String sheetName) {#insert-int-int-java.lang.String-}
```
public Worksheet insert(int index, int sheetType, String sheetName)
```


Inserisci un foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | L'indice del foglio |
| sheetType | int | [SheetType](../../com.aspose.cells/sheettype). Il tipo di foglio. |
| sheetName | java.lang.String | Il nome del foglio. |

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet) - Returns an inserted worksheet.
### isRefreshAllConnections() {#isRefreshAllConnections--}
```
public boolean isRefreshAllConnections()
```


Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase.

**Returns:**
java.util.Iterator - Un iteratore per l'istanza di CollectionBase.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshAll() {#refreshAll--}
```
public void refreshAll()
```


Aggiorna tutte le tabelle pivot e i grafici con la sorgente pivot.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare il metodo Workbook.RefreshAll(). Questo metodo sarà rimosso 12 mesi dopo, a partire da aprile 2026. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

### refreshPivotTables() {#refreshPivotTables--}
```
public void refreshPivotTables()
```


Aggiorna tutte le PivotTable nel file Excel.

### refreshPivotTables(PivotTableRefreshOption option) {#refreshPivotTables-com.aspose.cells.PivotTableRefreshOption-}
```
public boolean refreshPivotTables(PivotTableRefreshOption option)
```


Aggiorna tutte le PivotTable nel file Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | L'opzione per aggiornare la fonte dati delle tabelle pivot. |

**Returns:**
boolean
### registerAddInFunction(int id, String functionName) {#registerAddInFunction-int-java.lang.String-}
```
public String registerAddInFunction(int id, String functionName)
```


Aggiunge la funzione add-in nella cartella di lavoro

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| id | int | ID dei dati che contengono le funzioni add-in, può essere ottenuto dalla prima chiamata di [registerAddInFunction(String,String,boolean)](../../com.aspose.cells/worksheetcollection\#registerAddInFunction-String-String-boolean-) per lo stesso file add-in. |
| functionName | java.lang.String | il nome della funzione add-in |

**Returns:**
java.lang.String - URL del file add-in che contiene le funzioni add-in
### registerAddInFunction(String addInFile, String functionName, boolean lib) {#registerAddInFunction-java.lang.String-java.lang.String-boolean-}
```
public int registerAddInFunction(String addInFile, String functionName, boolean lib)
```


Aggiunge la funzione add-in nella cartella di lavoro

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| addInFile | java.lang.String | il file contiene le funzioni add-in |
| functionName | java.lang.String | il nome della funzione add-in |
| lib | boolean | se il file add-in fornito si trova nella directory o sottodirectory della libreria Workbook Add-In. Questa flag entra in vigore e fa differenza quando il file addInFile è di percorso relativo: true indica che il percorso è relativo alla libreria Add-In e false indica che il percorso è relativo a questo Workbook. |

**Returns:**
int - ID dei dati che contengono la funzione add-in fornita
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Rimuove l'elemento a un indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | Il valore indice dell'elemento da rimuovere. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Rimuove l'elemento a un nome specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String | Il nome dell'elemento da rimuovere. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Rappresenta l'indice del foglio di lavoro attivo quando il foglio di calcolo è aperto.

**Remarks**

L'indice del foglio è basato su zero.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setActiveSheetName(String value) {#setActiveSheetName-java.lang.String-}
```
public void setActiveSheetName(String value)
```


Rappresenta il nome del foglio di lavoro attivo quando il foglio di calcolo è aperto.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.String |  |

### setOleSize(int startRow, int endRow, int startColumn, int endColumn) {#setOleSize-int-int-int-int-}
```
public void setOleSize(int startRow, int endRow, int startColumn, int endColumn)
```


Imposta la dimensione visualizzata quando il file Cartella di lavoro è usato come oggetto OLE.

**Remarks**

Questo metodo è generalmente usato per regolare la dimensione di visualizzazione in un file ppt o doc.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| startRow | int | Indice della riga di inizio. |
| endRow | int | Indice della riga finale. |
| startColumn | int | Indice della colonna di inizio. |
| endColumn | int | Indice della colonna finale. |

### setOleSize(Object value) {#setOleSize-java.lang.Object-}
```
public void setOleSize(Object value)
```


Imposta la dimensione visualizzata quando il file Cartella di lavoro è usato come oggetto OLE.

**Remarks**

Null indica nessuna impostazione di dimensione ole.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | java.lang.Object |  |

### setRefreshAllConnections(boolean value) {#setRefreshAllConnections-boolean-}
```
public void setRefreshAllConnections(boolean value)
```


Indica se aggiornare tutte le connessioni all'apertura del file in MS Excel.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setXmlMaps(XmlMapCollection value) {#setXmlMaps-com.aspose.cells.XmlMapCollection-}
```
public void setXmlMaps(XmlMapCollection value)
```


Imposta le mappe XML nella cartella di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [XmlMapCollection](../../com.aspose.cells/xmlmapcollection) |  |

### sortNames() {#sortNames--}
```
public void sortNames()
```


Ordina i nomi definiti.

**Remarks**

Se crei un gran numero di intervalli denominati nel file Excel, chiama questo metodo dopo che tutti gli intervalli denominati sono stati creati e prima di salvare.

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


Scambia i due fogli.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sheetIndex1 | int | Il primo foglio di lavoro. |
| sheetIndex2 | int | Il secondo foglio di lavoro. |

### toString() {#toString--}
```
public String toString()
```




**Returns:**
java.lang.String
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

