---
title: "PivotTableCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la raccolta di tutti gli oggetti PivotTable nel foglio di lavoro specificato."
type: docs
url: /it/java/com.aspose.cells/pivottablecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotTableCollection extends CollectionBase
```

Rappresenta la raccolta di tutti gli oggetti PivotTable nel foglio di lavoro specificato.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         //Change PivotField's attributes
         PivotField rowField = pivot.getRowFields().get(0);
         rowField.setDisplayName("custom display name");
 
         //Add PivotFilter
         PivotFilter filter = pivot.getRowFields().get(0).filterTop10(0, PivotFilterType.PERCENT, false, 2);
 
 
         //Add PivotFormatCondition
         int formatIndex = pivot.getConditionalFormats().add();
         PivotConditionalFormat pfc = pivot.getConditionalFormats().get(formatIndex);
         pfc.addCellArea(pivot.getDataBodyRange());
         FormatConditionCollection fcc = pfc.getFormatConditions();
         int ii = fcc.addCondition(FormatConditionType.CELL_VALUE, OperatorType.GREATER_OR_EQUAL, "100", null);
 
         FormatCondition fc = fcc.get(ii);
 
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(PivotTable pivotTable, int row, int column, String tableName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Aggiunge una nuova PivotTable basata su un'altra PivotTable. |
| [add(PivotTable pivotTable, String destCellName, String tableName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Aggiunge una nuova PivotTable basata su un'altra PivotTable. |
| [add(Object o)](#add-java.lang.Object-) | Aggiunge un elemento all'istanza di CollectionBase. |
| [add(String sourceData, int row, int column)](#add-java.lang.String-int-int-) | Aggiunge una nuova PivotTable moderna (da Excel 2007) nella riga e colonna specificate del foglio di lavoro con le opzioni predefinite. |
| [add(String sourceData, int row, int column, PivotTableCreateOptions options)](#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-) | Aggiunge una nuova PivotTable nella riga e colonna specificate del foglio di lavoro. |
| [add(String sourceData, int row, int column, String tableName)](#add-java.lang.String-int-int-java.lang.String-) | Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource)](#add-java.lang.String-int-int-java.lang.String-boolean-) | Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003. |
| [add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-int-int-java.lang.String-boolean-boolean-) | Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003. |
| [add(String sourceData, String cellName)](#add-java.lang.String-java.lang.String-) | Aggiunge una nuova PivotTable moderna (da Excel 2007) nella riga e colonna specificate del foglio di lavoro con le opzioni predefinite. |
| [add(String sourceData, String cellName, PivotTableCreateOptions options)](#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-) | Aggiunge una nuova PivotTable moderna (da Excel 2007) nella riga e colonna specificate del foglio di lavoro con le opzioni predefinite. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003. |
| [add(String sourceData, String destCellName, String tableName, boolean useSameSource)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-) | Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003. |
| [add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)](#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-) | Aggiunge una nuova PivotTable. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-) | Aggiunge un nuovo oggetto PivotTable alla collezione con più intervalli di consolidamento come origine dati. |
| [add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)](#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-) | Aggiunge un nuovo oggetto PivotTable alla collezione con più intervalli di consolidamento come origine dati. |
| [clear()](#clear--) | Cancella tutte le tabelle pivot. |
| [contains(Object o)](#contains-java.lang.Object-) | Restituisce se l'istanza contiene questo oggetto |
| [dispose()](#dispose--) | Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene il report della PivotTable per indice. |
| [get(int row, int column)](#get-int-int-) | Ottiene la [PivotTable](../../com.aspose.cells/pivottable) situata nella cella. |
| [get(String name)](#get-java.lang.String-) | Ottiene il report della PivotTable per nome. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il numero di elementi contenuti nell'istanza di CollectionBase. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Determina l'indice di un elemento specifico nell'istanza di CollectionBase. |
| [iterator()](#iterator--) | Restituisce un enumeratore che itera attraverso l'istanza di CollectionBase. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(PivotTable pivotTable)](#remove-com.aspose.cells.PivotTable-) | Elimina la PivotTable specificata e rimuove i dati della PivotTable. |
| [remove(PivotTable pivotTable, boolean keepData)](#remove-com.aspose.cells.PivotTable-boolean-) | Elimina la PivotTable specificata. |
| [removeAt(int index)](#removeAt-int-) | Elimina la PivotTable all'indice specificato e rimuove i dati della PivotTable. |
| [removeAt(int index, boolean keepData)](#removeAt-int-boolean-) | Elimina la PivotTable all'indice specificato. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivotTable, int row, int column, String tableName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivotTable, int row, int column, String tableName)
```


Aggiunge una nuova PivotTable basata su un'altra PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | La PivotTable di origine. |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice della PivotTable appena aggiunta.
### add(PivotTable pivotTable, String destCellName, String tableName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivotTable, String destCellName, String tableName)
```


Aggiunge una nuova PivotTable basata su un'altra PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | La PivotTable di origine. |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice della PivotTable appena aggiunta.
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
### add(String sourceData, int row, int column) {#add-java.lang.String-int-int-}
```
public PivotTable add(String sourceData, int row, int column)
```


Aggiunge una nuova PivotTable moderna (da Excel 2007) nella riga e colonna specificate del foglio di lavoro con le opzioni predefinite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| riga | int | L'indice di riga basato su zero dell'angolo in alto a sinistra per la destinazione della PivotTable. |
| colonna | int | L'indice di colonna basato su zero dell'angolo in alto a sinistra per la destinazione della PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, PivotTableCreateOptions options) {#add-java.lang.String-int-int-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, int row, int column, PivotTableCreateOptions options)
```


Aggiunge una nuova PivotTable nella riga e colonna specificate del foglio di lavoro.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| riga | int | L'indice di riga basato su zero dell'angolo in alto a sinistra per la destinazione della PivotTable. |
| colonna | int | L'indice di colonna basato su zero dell'angolo in alto a sinistra per la destinazione della PivotTable. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Opzioni di creazione della PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, int row, int column, String tableName) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String sourceData, int row, int column, String tableName)
```


Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

**Remarks**

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo settembre 2026. Ci scusiamo per eventuali disagi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice in questo elenco di pivot table.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource) {#add-java.lang.String-int-int-java.lang.String-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource)
```


Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

**Remarks**

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo settembre 2026. Ci scusiamo per eventuali disagi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |
| useSameSource | boolean | Indica se utilizzare la stessa origine dati quando un'altra pivot table esistente ha già utilizzato questa origine dati. Se la proprietà è true, verrà risparmiata memoria. |

**Returns:**
int - L'indice della cache appena aggiunta.
### add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-int-int-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, int row, int column, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

**Remarks**

NOTE: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare l'overload PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) invece. Questo metodo sarà rimosso 12 mesi dopo ottobre 2026. Ci scusiamo per qualsiasi inconveniente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |
| useSameSource | boolean | Indica se utilizzare la stessa origine dati quando un'altra pivot table esistente ha già utilizzato questa origine dati. Se la proprietà è true, verrà risparmiata memoria. |
| isXlsClassic | boolean | Indica se aggiungere una tabella pivot classica di Excel 97-2003. |

**Returns:**
int - L'indice della cache appena aggiunta.
### add(String sourceData, String cellName) {#add-java.lang.String-java.lang.String-}
```
public PivotTable add(String sourceData, String cellName)
```


Aggiunge una nuova PivotTable moderna (da Excel 2007) nella riga e colonna specificate del foglio di lavoro con le opzioni predefinite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| cellName | java.lang.String | Il nome della cella in alto a sinistra per la destinazione della PivotTable. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String cellName, PivotTableCreateOptions options) {#add-java.lang.String-java.lang.String-com.aspose.cells.PivotTableCreateOptions-}
```
public PivotTable add(String sourceData, String cellName, PivotTableCreateOptions options)
```


Aggiunge una nuova PivotTable moderna (da Excel 2007) nella riga e colonna specificate del foglio di lavoro con le opzioni predefinite.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| cellName | java.lang.String | Il nome della cella in alto a sinistra per la destinazione della PivotTable. |
| options | [PivotTableCreateOptions](../../com.aspose.cells/pivottablecreateoptions) | Le opzioni per la creazione della tabella pivot. |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable) - The newly created PivotTable instance.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

**Remarks**

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo settembre 2026. Ci scusiamo per eventuali disagi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | I dati per la nuova cache della PivotTable. |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice in questo elenco di pivot table.
### add(String sourceData, String destCellName, String tableName, boolean useSameSource) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-}
```
public int add(String sourceData, String destCellName, String tableName, boolean useSameSource)
```


Aggiunge una nuova PivotTable con layout e stile legacy di Excel 97-2003.

**Remarks**

NOTA: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare invece la sovraccarico PivotTableCollection.Add(string, int, int, PivotTableCreateOptions). Questo metodo sarà rimosso 12 mesi dopo settembre 2026. Ci scusiamo per eventuali disagi.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | I dati per la nuova cache della PivotTable. |
| destCellName | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |
| useSameSource | boolean | Indica se utilizzare la stessa origine dati quando un'altra pivot table esistente ha già utilizzato questa origine dati. Se la proprietà è true, verrà risparmiata memoria. |

**Returns:**
int - L'indice della cache appena aggiunta.
### add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic) {#add-java.lang.String-java.lang.String-java.lang.String-boolean-boolean-}
```
public int add(String sourceData, String cell, String tableName, boolean useSameSource, boolean isXlsClassic)
```


Aggiunge una nuova PivotTable.

**Remarks**

NOTE: Questo metodo è obsoleto. È equivalente a chiamare PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) con `NewPivotTableOptions.IsXlsClassic = true`. Si prega di utilizzare l'overload PivotTableCollection.Add(string, int, int, PivotTableCreateOptions) invece. Questo metodo sarà rimosso 12 mesi dopo ottobre 2026. Ci scusiamo per qualsiasi inconveniente.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String | L'intervallo di celle dati per la nuova PivotTable. Esempio: Sheet1!A1:C8 |
| cella | java.lang.String | La cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |
| useSameSource | boolean | Indica se utilizzare la stessa origine dati quando un'altra tabella pivot esistente ha già usato questa origine dati. Se la proprietà è true, risparmierà memoria quando la stessa origine dati è stata raccolta in una singola cache pivot. |
| isXlsClassic | boolean | Indica se aggiungere una tabella pivot classica di Excel 97-2003. |

**Returns:**
int - L'indice della cache appena aggiunta.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-int-int-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, int row, int column, String tableName)
```


Aggiunge un nuovo oggetto PivotTable alla collezione con più intervalli di consolidamento come origine dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String[] | Gli intervalli di consolidamento multipli, ad esempio \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Indica se creare automaticamente un unico campo pagina. Se true, il parametro pageFields successivo sarà ignorato |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Gli elementi del campo pagina della pivot. |
| riga | int | Indice di riga della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| colonna | int | Indice di colonna della cella nell'angolo in alto a sinistra dell'intervallo di destinazione del report della PivotTable. |
| tableName | java.lang.String | Il nome del nuovo report della PivotTable. |

**Returns:**
int - L'indice della PivotTable appena aggiunta.
### add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName) {#add-java.lang.String---boolean-com.aspose.cells.PivotPageFields-java.lang.String-java.lang.String-}
```
public int add(String[] sourceData, boolean isAutoPage, PivotPageFields pageFields, String destCellName, String tableName)
```


Aggiunge un nuovo oggetto PivotTable alla collezione con più intervalli di consolidamento come origine dati.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| sourceData | java.lang.String[] | Gli intervalli di consolidamento multipli, ad esempio \{"Sheet1!A1:C8","Sheet2!A1:B8"\} |
| isAutoPage | boolean | Indica se creare automaticamente un unico campo pagina. Se true, il parametro pageFields successivo sarà ignorato. |
| pageFields | [PivotPageFields](../../com.aspose.cells/pivotpagefields) | Gli elementi del campo pagina della pivot. |
| destCellName | java.lang.String | destCellName Il nome del nuovo report PivotTable. |
| tableName | java.lang.String | il nome del nuovo report PivotTable. |

**Returns:**
int - L'indice della PivotTable appena aggiunta.
### clear() {#clear--}
```
public void clear()
```


Cancella tutte le tabelle pivot.

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
### dispose() {#dispose--}
```
public void dispose()
```


Esegue attività definite dall'applicazione associate al rilascio, alla liberazione o al ripristino di risorse non gestite.

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
public PivotTable get(int index)
```


Ottiene il report della PivotTable per indice.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(int row, int column) {#get-int-int-}
```
public PivotTable get(int row, int column)
```


Ottiene la [PivotTable](../../com.aspose.cells/pivottable) situata nella cella.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| riga | int |  |
| colonna | int |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
### get(String name) {#get-java.lang.String-}
```
public PivotTable get(String name)
```


Ottiene il report della PivotTable per nome.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[PivotTable](../../com.aspose.cells/pivottable)
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




### remove(PivotTable pivotTable) {#remove-com.aspose.cells.PivotTable-}
```
public void remove(PivotTable pivotTable)
```


Elimina la PivotTable specificata e rimuove i dati della PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Oggetto PivotTable |

### remove(PivotTable pivotTable, boolean keepData) {#remove-com.aspose.cells.PivotTable-boolean-}
```
public void remove(PivotTable pivotTable, boolean keepData)
```


Elimina la PivotTable specificata.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| pivotTable | [PivotTable](../../com.aspose.cells/pivottable) | Oggetto PivotTable |
| keepData | boolean | Indica se conservare i dati della PivotTable |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Elimina la PivotTable all'indice specificato e rimuove i dati della PivotTable.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice di posizione nella collezione PivotTable |

### removeAt(int index, boolean keepData) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean keepData)
```


Elimina la PivotTable all'indice specificato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int | l'indice di posizione nella collezione PivotTable |
| keepData | boolean | Indica se conservare i dati della PivotTable |

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

