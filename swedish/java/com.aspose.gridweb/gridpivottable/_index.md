---
title: "GridPivotTable"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en PivotTable-rapport i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.gridweb/gridpivottable/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTable
```

Representerar en pivottabellsrapport på ett kalkylblad. PivotTable‑objektet är en medlem i samlingen [GridPivotTable](../../com.aspose.gridweb/gridpivottable). Samlingen PivotTables innehåller alla PivotTable‑objekt på en kontroll.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addFieldToArea(int fieldType, int baseFieldIndex)](#addFieldToArea-int-int-) | Lägger till fältet i det specifika området. |
| [addFieldToArea(int fieldType, String fieldName)](#addFieldToArea-int-java.lang.String-) | Lägger till fältet i det specifika området. |
| [calculateData()](#calculateData--) | Beräknar pivottabellens data till celler. |
| [clearAllFields()](#clearAllFields--) | rensa alla pivottfält. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [fields(int fieldType)](#fields-int-) | Hämtar de specifika fälten efter fälttypen. |
| [fields(String fieldName)](#fields-java.lang.String-) | Hämtar det specifika fältet efter fältnamnet. |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshData()](#refreshData--) | Uppdaterar pivottabellens data och inställningar från dess datakälla. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addFieldToArea(int fieldType, int baseFieldIndex) {#addFieldToArea-int-int-}
```
public int addFieldToArea(int fieldType, int baseFieldIndex)
```


Lägger till fältet i det specifika området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Typ av fältområde. |
| baseFieldIndex | int | Fältindexet i basfälten. |

**Returns:**
int - Fältets position i de specifika fälten.
### addFieldToArea(int fieldType, String fieldName) {#addFieldToArea-int-java.lang.String-}
```
public int addFieldToArea(int fieldType, String fieldName)
```


Lägger till fältet i det specifika området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). Typ av fältområde. |
| fieldName | java.lang.String | Namnet i basfälten. |

**Returns:**
int - Fältets position i de specifika fälten. Om det inte finns något fält med detta namn, returnera -1.
### calculateData() {#calculateData--}
```
public void calculateData()
```


Beräknar pivottabellens data till celler.

**Remarks**

Cell.Value i pivotrangen kan inte returnera korrekt resultat om metoden inte har anropats. Denna metod beräknar data med en intern pivottcache, inte den ursprungliga datakällan. Så om datakällan ändras, anropa först metoden RefreshData().

### clearAllFields() {#clearAllFields--}
```
public void clearAllFields()
```


rensa alla pivottfält.

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
### fields(int fieldType) {#fields-int-}
```
public GridPivotFieldCollection fields(int fieldType)
```


Hämtar de specifika fälten efter fälttypen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldType | int | [GridPivotFieldType](../../com.aspose.gridweb/gridpivotfieldtype). fälttypen. |

**Returns:**
[GridPivotFieldCollection](../../com.aspose.gridweb/gridpivotfieldcollection) - the specific fields
### fields(String fieldName) {#fields-java.lang.String-}
```
public GridPivotField fields(String fieldName)
```


Hämtar det specifika fältet efter fältnamnet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldName | java.lang.String | fältnamnet. |

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


Uppdaterar pivottabellens data och inställningar från dess datakälla.

**Remarks**

Vi samlar data från datakällan till en pivottcache, och beräknar sedan data i cachen till cellerna. Denna metod används endast för att samla all data i en pivottcache.

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

