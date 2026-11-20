---
title: "GridPivotTable"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta un report PivotTable su un foglio di lavoro."
type: docs
url: /it/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

Rappresenta un report PivotTable in un foglio di lavoro. L'oggetto PivotTable è un membro della collezione [GridPivotTable](../../com.aspose.gridweb/gridpivottable). La collezione PivotTables contiene tutti gli oggetti PivotTable su un controllo.
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Aggiunge il campo all'area specifica. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Aggiunge il campo all'area specifica. |
| [calculateData()](#calculateData--) | Calcola i dati della PivotTable nelle celle. |
| [clearAllFields()](#clearAllFields--) | Cancella tutti i campi pivot. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Ottiene i campi specifici per tipo di campo. |
| [fields(String fieldName)](#fields-java.lang.String-) | Ottiene il campo specifico per nome del campo. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | Aggiorna i dati e le impostazioni della PivotTable dalla sua origine dati. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Aggiunge il campo all'area specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Il tipo di area dei campi. |
| baseFieldIndex | int | L'indice del campo nei campi di base. |

**Returns:**
int - La posizione del campo nei campi specifici.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Aggiunge il campo all'area specifica.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Il tipo di area dei campi. |
| fieldName | java.lang.String | Il nome nei campi di base. |

**Returns:**
int - La posizione del campo nei campi specifici. Se non esiste alcun campo con quel nome, restituisce -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Calcola i dati della PivotTable nelle celle.

**Remarks**

Cell.Value nell'intervallo pivot potrebbe non restituire il risultato corretto se il metodo non è stato chiamato. Questo metodo calcola i dati con una cache pivot interna, non con la fonte dati originale. Quindi, se la fonte dati è cambiata, si prega di chiamare prima il metodo RefreshData().

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


Cancella tutti i campi pivot.

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


Ottiene i campi specifici per tipo di campo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). il tipo di campo. |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


Ottiene il campo specifico per nome del campo.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| fieldName | java.lang.String | il nome del campo. |

**Returns:**
[GridPivotField](../../com.aspose.gridweb/gridpivotfield) - the specific field
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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




### refreshData() {#refreshData--}
```
public void refreshData()
```


Aggiorna i dati e le impostazioni della PivotTable dalla sua origine dati.

**Remarks**

Raccoglieremo i dati dalla fonte dati in una cache pivot, quindi calcoleremo i dati nella cache nelle celle. Questo metodo è usato solo per raccogliere tutti i dati in una cache pivot.

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

