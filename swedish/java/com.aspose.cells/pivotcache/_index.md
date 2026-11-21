---
title: "PivotCache"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar minnescachen för vissa pivottabellsrapporter."
type: docs
url: /sv/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

Representerar minnescachen för vissa pivottabellsrapporter.

**Remarks**

All data kommer att samlas i den här cachen, och pivottabellen hämtar endast data från den här cachen, inte direkt från datakällan. Om datakällan för vissa [PivotTable](../../com.aspose.cells/pivottable)s är densamma, kommer de att använda en pivot cache.
## Konstruktörer

| Konstruktör | Beskrivning |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [dispose()](#dispose--) | Frigör alla resurser. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | Hämtar antalet oanvända objekt som tillåts innan oanvända objekt kastas. |
| [getPivotTables()](#getPivotTables--) | Hämtar alla pivottabeller med den här pivotcachen. |
| [getSourceType()](#getSourceType--) | Hämtar [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är den här pivotcachen. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är den här pivotcachen. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | Ställer in antalet oanvända objekt som tillåts innan oanvända objekt kastas. |
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


Frigör alla resurser.

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
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


Hämtar antalet oanvända objekt som tillåts innan oanvända objekt kastas. Detta värde MÅSTE vara större än -2 och mindre än 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


Hämtar alla pivottabeller med den här pivotcachen.

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


Hämtar [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

Se [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

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


Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är den här pivotcachen.

**Remarks**

Om både table1 och table2 använder den här cachen, kommer de två tabellerna att beräknas. Det är bättre att du helt enkelt kan anropa [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) för att uppdatera alla pivottabeller och diagram i filen.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


Uppdaterar data från datakällan och beräknar data för vyn av alla pivottabeller vars datakälla är den här pivotcachen.

**Remarks**

Det är bättre att du helt enkelt kan anropa [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) för att uppdatera alla pivottabeller och diagram i filen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | Alternativen för att uppdatera datakällan för pivottabellen. |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


Ställer in antalet oanvända objekt som tillåts innan oanvända objekt kastas. Detta värde MÅSTE vara större än -2 och mindre än 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

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

