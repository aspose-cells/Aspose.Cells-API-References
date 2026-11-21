---
title: "PivotTableCalculateOption"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att beräkna data i pivottabellen."
type: docs
url: /sv/java/com.aspose.cells/pivottablecalculateoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableCalculateOption
```

Representerar alternativen för att beräkna data i pivottabellen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PivotTableCalculateOption()](#PivotTableCalculateOption--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRefreshCharts()](#getRefreshCharts--) | Anger om uppdatering av diagram baseras på denna pivottabell. |
| [getRefreshData()](#getRefreshData--) | Anger om uppdatering av datakällan för pivottabellen. |
| [getRefreshOption()](#getRefreshOption--) | Hämtar alternativ för att uppdatera datakällan till pivottcache. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Representerar hur man reserverar saknade pivotelement. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setRefreshCharts(boolean value)](#setRefreshCharts-boolean-) | Anger om uppdatering av diagram baseras på denna pivottabell. |
| [setRefreshData(boolean value)](#setRefreshData-boolean-) | Anger om uppdatering av datakällan för pivottabellen. |
| [setRefreshOption(PivotTableRefreshOption value)](#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-) | Ställer in alternativ för att uppdatera datakällan till pivottcache. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Representerar hur man reserverar saknade pivotelement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableCalculateOption() {#PivotTableCalculateOption--}
```
public PivotTableCalculateOption()
```


### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
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
### getRefreshCharts() {#getRefreshCharts--}
```
public boolean getRefreshCharts()
```


Anger om uppdatering av diagram baseras på denna pivottabell.

**Returns:**
boolean
### getRefreshData() {#getRefreshData--}
```
public boolean getRefreshData()
```


Anger om uppdatering av datakällan för pivottabellen.

**Remarks**

Om den är sann, uppdatera pivottcachen från datakällan, och beräkna sedan alla pivottabeller baserat på samma pivottcache.

**Returns:**
boolean
### getRefreshOption() {#getRefreshOption--}
```
public PivotTableRefreshOption getRefreshOption()
```


Hämtar alternativ för att uppdatera datakällan till pivottcache.

**Returns:**
[PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption)
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Representerar hur man reserverar saknade pivotelement.

Se [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Fungerar endast när [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) är sann.

**Returns:**
int
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




### setRefreshCharts(boolean value) {#setRefreshCharts-boolean-}
```
public void setRefreshCharts(boolean value)
```


Anger om uppdatering av diagram baseras på denna pivottabell.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRefreshData(boolean value) {#setRefreshData-boolean-}
```
public void setRefreshData(boolean value)
```


Anger om uppdatering av datakällan för pivottabellen.

**Remarks**

Om den är sann, uppdatera pivottcachen från datakällan, och beräkna sedan alla pivottabeller baserat på samma pivottcache.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setRefreshOption(PivotTableRefreshOption value) {#setRefreshOption-com.aspose.cells.PivotTableRefreshOption-}
```
public void setRefreshOption(PivotTableRefreshOption value)
```


Ställer in alternativ för att uppdatera datakällan till pivottcache.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| value | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Representerar hur man reserverar saknade pivotelement.

Se [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

**Remarks**

Fungerar endast när [getRefreshData()](../../com.aspose.cells/pivottablecalculateoption\#getRefreshData--) är sann.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

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
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

