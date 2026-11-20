---
title: "FindOptions"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di ricerca."
type: docs
url: /it/java/com.aspose.cells/findoptions/
---

**Inheritance:**
java.lang.Object
```
public class FindOptions
```

Rappresenta le opzioni di ricerca.

**Example**

```
         //Instantiate the workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Get Cells collection 
         Cells cells = workbook.getWorksheets().get(0).getCells();
 
         //Instantiate FindOptions Object
         FindOptions findOptions = new FindOptions();
 
         //Create a Cells Area
         CellArea ca = new CellArea();
         ca.StartRow = 8;
         ca.StartColumn = 2;
         ca.EndRow = 17;
         ca.EndColumn = 13;
 
         //Set cells area for find options
         findOptions.setRange(ca);
 
         //Set searching properties
         findOptions.setSearchBackward(false);
 
         findOptions.setSearchOrderByRows(true);
 
         findOptions.setLookInType(LookInType.VALUES);
 
         //Find the cell with 0 value
         Cell cell = cells.find(0, null, findOptions);
```
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [FindOptions()](#FindOptions--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Indica se la stringa cercata è sensibile al maiuscolo/minuscolo. |
| [getClass()](#getClass--) |  |
| [getConvertNumericData()](#getConvertNumericData--) | Ottiene un valore che indica se convertire il valore della stringa cercata in dati numerici. |
| [getLookAtType()](#getLookAtType--) | Tipo di ricerca 'look at'. |
| [getLookInType()](#getLookInType--) | Tipo di ricerca 'look in'. |
| [getRange()](#getRange--) | Ottiene e imposta l'intervallo di ricerca. |
| [getRegexKey()](#getRegexKey--) | Indica se la chiave cercata è una regex. |
| [getSearchBackward()](#getSearchBackward--) | Se cercare all'indietro le celle. |
| [getSearchNext()](#getSearchNext--) | Ordine di ricerca. |
| [getSearchOrderByRows()](#getSearchOrderByRows--) | Indica se l'ordine di ricerca è per righe o colonne. |
| [getStyle()](#getStyle--) | Il formato da cercare. |
| [getValueTypeSensitive()](#getValueTypeSensitive--) | Indica se il tipo di valore della cella cercata deve essere lo stesso della chiave cercata. |
| [hashCode()](#hashCode--) |  |
| [isRangeSet()](#isRangeSet--) | Indica se l'intervallo cercato è impostato. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Indica se la stringa cercata è sensibile al maiuscolo/minuscolo. |
| [setConvertNumericData(boolean value)](#setConvertNumericData-boolean-) | Imposta un valore che indica se convertire il valore stringa cercato in dati numerici. |
| [setLookAtType(int value)](#setLookAtType-int-) | Tipo di ricerca 'look at'. |
| [setLookInType(int value)](#setLookInType-int-) | Tipo di ricerca 'look in'. |
| [setRange(CellArea ca)](#setRange-com.aspose.cells.CellArea-) | Imposta l'intervallo cercato. |
| [setRegexKey(boolean value)](#setRegexKey-boolean-) | Indica se la chiave cercata è una regex. |
| [setSearchBackward(boolean value)](#setSearchBackward-boolean-) | Se cercare all'indietro le celle. |
| [setSearchNext(boolean value)](#setSearchNext-boolean-) | Ordine di ricerca. |
| [setSearchOrderByRows(boolean value)](#setSearchOrderByRows-boolean-) | Indica se l'ordine di ricerca è per righe o colonne. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | Il formato da cercare. |
| [setValueTypeSensitive(boolean value)](#setValueTypeSensitive-boolean-) | Indica se il tipo di valore della cella cercata deve essere lo stesso della chiave cercata. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### FindOptions() {#FindOptions--}
```
public FindOptions()
```


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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Indica se la stringa cercata è sensibile al maiuscolo/minuscolo.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getConvertNumericData() {#getConvertNumericData--}
```
public boolean getConvertNumericData()
```


Ottiene un valore che indica se convertire il valore della stringa cercata in dati numerici.

**Returns:**
boolean
### getLookAtType() {#getLookAtType--}
```
public int getLookAtType()
```


Tipo di ricerca 'look at'.

Vedi [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Quando [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) è true e l'utente ha specificato la regola esatta per la regex, per motivi di prestazioni questa proprietà dovrebbe essere impostata su [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). Altrimenti riformuleremo la chiave di ricerca per garantire che possa essere corrisposta secondo il tipo specifico. Ad esempio, quando il tipo è [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (questo è il valore predefinito per questa proprietà), aggiungeremo automaticamente i caratteri jolly all'inizio e alla fine della chiave di ricerca. In questo caso, le espressioni regolari diventeranno più complesse e le prestazioni diminuiranno.

**Returns:**
int
### getLookInType() {#getLookInType--}
```
public int getLookInType()
```


Tipo di ricerca 'look in'.

Vedi [LookInType](../../com.aspose.cells/lookintype).

**Returns:**
int
### getRange() {#getRange--}
```
public CellArea getRange()
```


Ottiene e imposta l'intervallo di ricerca.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Returns the searched range.
### getRegexKey() {#getRegexKey--}
```
public boolean getRegexKey()
```


Indica se la chiave cercata è una regex. Se true la chiave cercata verrà considerata come regex e analizzata. Altrimenti la chiave verrà analizzata secondo le regole di MS Excel.

**Remarks**

Anche se la chiave di ricerca è stata specificata come regex, potrebbe essere riformulata in base a [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--). Ad esempio, quando il tipo è [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (questo è il valore predefinito per queste opzioni), i caratteri jolly verranno aggiunti automaticamente all'inizio e alla fine della chiave di ricerca per garantire che la corrispondenza venga verificata come \"contains\". In questo caso, le espressioni regolari diventeranno più complesse e le prestazioni diminuiranno. Pertanto, per motivi di prestazioni, se l'utente ha specificato la regola esatta per la regex, non è necessario utilizzare [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) come vincolo aggiuntivo e l'utente può impostarlo su [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) per ottenere migliori prestazioni.

**Returns:**
boolean
### getSearchBackward() {#getSearchBackward--}
```
public boolean getSearchBackward()
```


Se cercare all'indietro le celle.

**Returns:**
boolean
### getSearchNext() {#getSearchNext--}
```
public boolean getSearchNext()
```


Ordine di ricerca. True: cerca il successivo. False: cerca il precedente.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FindOptions.SearchBackward. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2018. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Returns:**
boolean
### getSearchOrderByRows() {#getSearchOrderByRows--}
```
public boolean getSearchOrderByRows()
```


Indica se l'ordine di ricerca è per righe o colonne.

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


Il formato da cercare.

**Returns:**
[Style](../../com.aspose.cells/style)
### getValueTypeSensitive() {#getValueTypeSensitive--}
```
public boolean getValueTypeSensitive()
```


Indica se il tipo di valore della cella cercata deve essere lo stesso della chiave cercata.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRangeSet() {#isRangeSet--}
```
public boolean isRangeSet()
```


Indica se l'intervallo cercato è impostato.

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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Indica se la stringa cercata è sensibile al maiuscolo/minuscolo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setConvertNumericData(boolean value) {#setConvertNumericData-boolean-}
```
public void setConvertNumericData(boolean value)
```


Imposta un valore che indica se convertire il valore stringa cercato in dati numerici.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setLookAtType(int value) {#setLookAtType-int-}
```
public void setLookAtType(int value)
```


Tipo di ricerca 'look at'.

Vedi [LookAtType](../../com.aspose.cells/lookattype).

**Remarks**

Quando [getRegexKey()](../../com.aspose.cells/findoptions\#getRegexKey--) è true e l'utente ha specificato la regola esatta per la regex, per motivi di prestazioni questa proprietà dovrebbe essere impostata su [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT). Altrimenti riformuleremo la chiave di ricerca per garantire che possa essere corrisposta secondo il tipo specifico. Ad esempio, quando il tipo è [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (questo è il valore predefinito per questa proprietà), aggiungeremo automaticamente i caratteri jolly all'inizio e alla fine della chiave di ricerca. In questo caso, le espressioni regolari diventeranno più complesse e le prestazioni diminuiranno.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setLookInType(int value) {#setLookInType-int-}
```
public void setLookInType(int value)
```


Tipo di ricerca 'look in'.

Vedi [LookInType](../../com.aspose.cells/lookintype).

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | int |  |

### setRange(CellArea ca) {#setRange-com.aspose.cells.CellArea-}
```
public void setRange(CellArea ca)
```


Imposta l'intervallo cercato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | l'intervallo cercato. |

### setRegexKey(boolean value) {#setRegexKey-boolean-}
```
public void setRegexKey(boolean value)
```


Indica se la chiave cercata è una regex. Se true la chiave cercata verrà considerata come regex e analizzata. Altrimenti la chiave verrà analizzata secondo le regole di MS Excel.

**Remarks**

Anche se la chiave di ricerca è stata specificata come regex, potrebbe essere riformulata in base a [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--). Ad esempio, quando il tipo è [LookAtType.CONTAINS](../../com.aspose.cells/lookattype\#CONTAINS) (questo è il valore predefinito per queste opzioni), i caratteri jolly verranno aggiunti automaticamente all'inizio e alla fine della chiave di ricerca per garantire che la corrispondenza venga verificata come \"contains\". In questo caso, le espressioni regolari diventeranno più complesse e le prestazioni diminuiranno. Pertanto, per motivi di prestazioni, se l'utente ha specificato la regola esatta per la regex, non è necessario utilizzare [getLookAtType()](../../com.aspose.cells/findoptions\#getLookAtType--) come vincolo aggiuntivo e l'utente può impostarlo su [LookAtType.ENTIRE\_CONTENT](../../com.aspose.cells/lookattype\#ENTIRE-CONTENT) per ottenere migliori prestazioni.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSearchBackward(boolean value) {#setSearchBackward-boolean-}
```
public void setSearchBackward(boolean value)
```


Se cercare all'indietro le celle.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSearchNext(boolean value) {#setSearchNext-boolean-}
```
public void setSearchNext(boolean value)
```


Ordine di ricerca. True: cerca il successivo. False: cerca il precedente.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, si prega di utilizzare la proprietà FindOptions.SearchBackward. Questa proprietà sarà rimossa 12 mesi dopo, a partire da novembre 2018. Aspose si scusa per eventuali disagi che potresti aver riscontrato.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setSearchOrderByRows(boolean value) {#setSearchOrderByRows-boolean-}
```
public void setSearchOrderByRows(boolean value)
```


Indica se l'ordine di ricerca è per righe o colonne.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


Il formato da cercare.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setValueTypeSensitive(boolean value) {#setValueTypeSensitive-boolean-}
```
public void setValueTypeSensitive(boolean value)
```


Indica se il tipo di valore della cella cercata deve essere lo stesso della chiave cercata.

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

