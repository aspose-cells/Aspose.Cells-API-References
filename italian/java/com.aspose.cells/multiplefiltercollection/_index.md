---
title: "MultipleFilterCollection"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta la collezione di filtri multipli."
type: docs
url: /it/java/com.aspose.cells/multiplefiltercollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class MultipleFilterCollection implements Iterable
```

Rappresenta la collezione di filtri multipli.

**Remarks**

NOTA: Questa classe è ora obsoleta. Invece, utilizzare [FilterValueCollection](../../com.aspose.cells/filtervaluecollection). Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2026. Aspose si scusa per eventuali disagi subiti.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [MultipleFilterCollection()](#MultipleFilterCollection--) | Crea una nuova istanza. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [add(int type, int year, int month, int day)](#add-int-int-int-int-) | Aggiunge un valore di criterio di filtro data. |
| [add(int type, int year, int month, int day, int hour, int minute, int second)](#add-int-int-int-int-int-int-int-) | Aggiunge un valore di criterio di filtro data e ora. |
| [add(String filter)](#add-java.lang.String-) | Aggiunge un criterio di filtro etichetta. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Ottiene [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) o un valore stringa. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ottiene il conteggio dei valori del filtro. |
| [getMatchBlank()](#getMatchBlank--) | Indica se filtrare per vuoto. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Ottieni l'enumeratore per il valore del filtro, |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setMatchBlank(boolean value)](#setMatchBlank-boolean-) | Indica se filtrare per vuoto. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### MultipleFilterCollection() {#MultipleFilterCollection--}
```
public MultipleFilterCollection()
```


Crea una nuova istanza.

**Remarks**

NOTA: Questo membro è ora obsoleto. Invece, impostare FilterColumn.FilterType su FilterType.MultipleFilters quindi ottenere FilterColumn.MultipleFilters. Questa proprietà sarà rimossa 12 mesi dopo, a partire da giugno 2026. Aspose si scusa per eventuali disagi subiti.

### add(int type, int year, int month, int day) {#add-int-int-int-int-}
```
public void add(int type, int year, int month, int day)
```


Aggiunge un valore di criterio di filtro data.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Il tipo di filtro data. |
| anno | int | L'anno. |
| mese | int | Il mese. |
| giorno | int | Il giorno. |

### add(int type, int year, int month, int day, int hour, int minute, int second) {#add-int-int-int-int-int-int-int-}
```
public void add(int type, int year, int month, int day, int hour, int minute, int second)
```


Aggiunge un valore di criterio di filtro data e ora.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| type | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). Il tipo di filtro data. |
| anno | int | L'anno. |
| mese | int | Il mese. |
| giorno | int | Il giorno. |
| ora | int | L'ora. |
| minuto | int | Il minuto. |
| secondo | int | Il secondo. |

### add(String filter) {#add-java.lang.String-}
```
public void add(String filter)
```


Aggiunge un criterio di filtro etichetta.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| filter | java.lang.String | I dati del filtro. |

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
public Object get(int index)
```


Ottiene [DateTimeGroupItem](../../com.aspose.cells/datetimegroupitem) o un valore stringa.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| indice | int |  |

**Returns:**
java.lang.Object -
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


Ottiene il conteggio dei valori del filtro.

**Returns:**
int
### getMatchBlank() {#getMatchBlank--}
```
public boolean getMatchBlank()
```


Indica se filtrare per vuoto.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Ottieni l'enumeratore per il valore del filtro,

**Returns:**
java.util.Iterator -
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setMatchBlank(boolean value) {#setMatchBlank-boolean-}
```
public void setMatchBlank(boolean value)
```


Indica se filtrare per vuoto.

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

