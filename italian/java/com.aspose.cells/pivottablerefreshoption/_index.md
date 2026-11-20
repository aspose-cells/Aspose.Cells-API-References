---
title: "PivotTableRefreshOption"
second_title: "Riferimento API di Aspose.Cells per Java"
description: "Rappresenta le opzioni di aggiornamento della fonte dati della PivotTable."
type: docs
url: /it/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

Rappresenta le opzioni di aggiornamento della fonte dati della PivotTable.
## Costruttori

| Costruttore | Descrizione |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | Rappresenta le opzioni di aggiornamento della fonte dati della PivotTable. |
## Metodi

| Metodo | Descrizione |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | Indica se mantenere i dati di gruppo locali nella cache se i valori massimo e minimo rimangono invariati. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Rappresenta come riservare gli elementi pivot mancanti. |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | Indica se mantenere l'ordine originale degli elementi pivot come nella vecchia origine dati. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | Indica se mantenere i dati di gruppo locali nella cache se i valori massimo e minimo rimangono invariati. |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | Indica se mantenere l'ordine originale degli elementi pivot come nella vecchia origine dati. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Rappresenta come riservare gli elementi pivot mancanti. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


Rappresenta le opzioni di aggiornamento della fonte dati della PivotTable.

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


Indica se mantenere i dati di gruppo locali nella cache se i valori massimo e minimo rimangono invariati. Il valore predefinito è false, il che significa aggiornare il gruppo con impostazione locale.

**Remarks**

Questa è una soluzione temporanea, si prega di localizzare le tabelle pivot implementando [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Rappresenta come riservare gli elementi pivot mancanti.

Vedi [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isKeepOriginalOrder() {#isKeepOriginalOrder--}
```
public boolean isKeepOriginalOrder()
```


Indica se mantenere l'ordine originale degli elementi pivot come nella vecchia origine dati.

**Remarks**

Applicabile solo al campo pivot che non è ordinato. Quando si aggiorna questo tipo di campo pivot, Ms Excel mantiene l'ordine originale della vecchia origine dati. Il valore predefinito di questa proprietà è true, rappresentando lo stesso comportamento di Ms Excel. Se l'utente necessita che il campo pivot venga aggiornato completamente come i dati nella nuova origine dati, questa proprietà dovrebbe essere impostata su false.

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




### setKeepCachedLocalGroupData(boolean value) {#setKeepCachedLocalGroupData-boolean-}
```
public void setKeepCachedLocalGroupData(boolean value)
```


Indica se mantenere i dati di gruppo locali nella cache se i valori massimo e minimo rimangono invariati. Il valore predefinito è false, il che significa aggiornare il gruppo con impostazione locale.

**Remarks**

Questa è una soluzione temporanea, si prega di localizzare le tabelle pivot implementando [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


Indica se mantenere l'ordine originale degli elementi pivot come nella vecchia origine dati.

**Remarks**

Applicabile solo al campo pivot che non è ordinato. Quando si aggiorna questo tipo di campo pivot, Ms Excel mantiene l'ordine originale della vecchia origine dati. Il valore predefinito di questa proprietà è true, rappresentando lo stesso comportamento di Ms Excel. Se l'utente necessita che il campo pivot venga aggiornato completamente come i dati nella nuova origine dati, questa proprietà dovrebbe essere impostata su false.

**Parameters:**
| Parametro | Tipo | Descrizione |
| --- | --- | --- |
| valore | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Rappresenta come riservare gli elementi pivot mancanti.

Vedi [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

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

