---
title: "PivotCache"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la cache di memoria per alcuni report PivotTable."
type: docs
url: /it/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

Rappresenta la cache di memoria per alcuni report PivotTable.

**Remarks**

Tutti i dati saranno raccolti in questa cache, e la tabella pivot otterrà i dati solo da questa cache, non accedendo direttamente alla fonte dati. Se la fonte dati di alcune [PivotTable](../../com.aspose.cells/pivottable)s è la stessa, utilizzeranno una cache pivot.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [dispose()](#dispose--) | Rilascia tutte le risorse. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Restituisce il numero di elementi inutilizzati da consentire prima di scartarli. |
| [getPivotTables()](#getPivotTables--) | Restituisce tutte le tabelle pivot con questa cache pivot. |
| [getSourceType()](#getSourceType--) | Restituisce il [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le tabelle pivot la cui fonte dati è questa cache pivot. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le tabelle pivot la cui fonte dati è questa cache pivot. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Imposta il numero di elementi inutilizzati da consentire prima di scartarli. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotCache() {#PivotCache--}
```
public PivotCache()
```


### dispose() {#dispose--}
```
public abstract void dispose()
```


Rilascia tutte le risorse.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Restituisce il numero di elementi inutilizzati da consentire prima di scartarli. Questo valore DEVE essere maggiore di -2 e minore di 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


Restituisce tutte le tabelle pivot con questa cache pivot.

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


Restituisce il [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

Vedi [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refresh() {#refresh--}
```
public int refresh()
```


Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le tabelle pivot la cui fonte dati è questa cache pivot.

**Remarks**

Se sia table1 che table2 utilizzano questa cache, le due tabelle verranno calcolate. È consigliabile chiamare semplicemente [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) per aggiornare tutte le tabelle pivot e i grafici nel file.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Aggiorna i dati dalla fonte dati e calcola i dati per la visualizzazione di tutte le tabelle pivot la cui fonte dati è questa cache pivot.

**Remarks**

È consigliabile chiamare semplicemente [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) per aggiornare tutte le tabelle pivot e i grafici nel file.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Le opzioni per l'aggiornamento della fonte dati della tabella pivot. |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Imposta il numero di elementi inutilizzati da consentire prima di scartarli. Questo valore DEVE essere maggiore di -2 e minore di 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

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

