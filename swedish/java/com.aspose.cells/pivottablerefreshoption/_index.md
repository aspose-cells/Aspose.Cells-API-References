---
title: "PivotTableRefreshOption"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alternativen för att uppdatera datakällan för pivottabellen."
type: docs
url: /sv/java/com.aspose.cells/pivottablerefreshoption/
---

**Inheritance:**
java.lang.Object
```
public class PivotTableRefreshOption
```

Representerar alternativen för att uppdatera datakällan för pivottabellen.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PivotTableRefreshOption()](#PivotTableRefreshOption--) | Representerar alternativen för att uppdatera datakällan för pivottabellen. |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getKeepCachedLocalGroupData()](#getKeepCachedLocalGroupData--) | Anger om cachad lokal gruppdata ska behållas om de maximala och minimala värdena förblir oförändrade. |
| [getReserveMissingPivotItemType()](#getReserveMissingPivotItemType--) | Representerar hur man reserverar saknade pivotelement. |
| [hashCode()](#hashCode--) |  |
| [isKeepOriginalOrder()](#isKeepOriginalOrder--) | Anger om pivotelementens ursprungliga ordning ska behållas som i den gamla datakällan. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setKeepCachedLocalGroupData(boolean value)](#setKeepCachedLocalGroupData-boolean-) | Anger om cachad lokal gruppdata ska behållas om de maximala och minimala värdena förblir oförändrade. |
| [setKeepOriginalOrder(boolean value)](#setKeepOriginalOrder-boolean-) | Anger om pivotelementens ursprungliga ordning ska behållas som i den gamla datakällan. |
| [setReserveMissingPivotItemType(int value)](#setReserveMissingPivotItemType-int-) | Representerar hur man reserverar saknade pivotelement. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotTableRefreshOption() {#PivotTableRefreshOption--}
```
public PivotTableRefreshOption()
```


Representerar alternativen för att uppdatera datakällan för pivottabellen.

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
### getKeepCachedLocalGroupData() {#getKeepCachedLocalGroupData--}
```
public boolean getKeepCachedLocalGroupData()
```


Anger om cachad lokal gruppdata ska behållas om de maximala och minimala värdena förblir oförändrade. Standardvärdet är false, vilket betyder att gruppen uppdateras med lokal inställning.

**Remarks**

Detta är en tillfällig lösning, vänligen lokalisera pivottabeller genom att implementera [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Returns:**
boolean
### getReserveMissingPivotItemType() {#getReserveMissingPivotItemType--}
```
public int getReserveMissingPivotItemType()
```


Representerar hur man reserverar saknade pivotelement.

Se [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

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


Anger om pivotelementens ursprungliga ordning ska behållas som i den gamla datakällan.

**Remarks**

Endast tillämplig för pivottfältet som inte är sorterat. Vid uppdatering av en sådan pivottfält behåller Ms Excel den ursprungliga ordningen för den gamla datakällan. Standardvärdet för denna egenskap är true, vilket representerar samma beteende som Ms Excel. Om användaren behöver att pivottfältet uppdateras helt enligt data i den nya datakällan, bör denna egenskap sättas till false.

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


Anger om cachad lokal gruppdata ska behållas om de maximala och minimala värdena förblir oförändrade. Standardvärdet är false, vilket betyder att gruppen uppdateras med lokal inställning.

**Remarks**

Detta är en tillfällig lösning, vänligen lokalisera pivottabeller genom att implementera [PivotGlobalizationSettings](../../com.aspose.cells/pivotglobalizationsettings)

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setKeepOriginalOrder(boolean value) {#setKeepOriginalOrder-boolean-}
```
public void setKeepOriginalOrder(boolean value)
```


Anger om pivotelementens ursprungliga ordning ska behållas som i den gamla datakällan.

**Remarks**

Endast tillämplig för pivottfältet som inte är sorterat. Vid uppdatering av en sådan pivottfält behåller Ms Excel den ursprungliga ordningen för den gamla datakällan. Standardvärdet för denna egenskap är true, vilket representerar samma beteende som Ms Excel. Om användaren behöver att pivottfältet uppdateras helt enligt data i den nya datakällan, bör denna egenskap sättas till false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setReserveMissingPivotItemType(int value) {#setReserveMissingPivotItemType-int-}
```
public void setReserveMissingPivotItemType(int value)
```


Representerar hur man reserverar saknade pivotelement.

Se [ReserveMissingPivotItemType](../../com.aspose.cells/reservemissingpivotitemtype).

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

