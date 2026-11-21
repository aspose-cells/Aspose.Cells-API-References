---
title: "GridPivotTableCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Inkapslar en samling av objekt."
type: docs
url: /sv/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

Inkapslar en samling av [GridPivotTable](../../com.aspose.gridweb/gridpivottable)-objekt.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Lägger till en ny PivotTable-cache i en PivotCaches-samling. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | Lägger till en ny PivotTable-cache i en PivotCaches-samling. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | Lägger till en ny PivotTable-cache i en PivotCaches-samling. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | Lägger till en ny PivotTable-cache i en PivotCaches-samling. |
| [clear()](#clear--) | Rensar alla PivotTables. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar [GridPivotTable](../../com.aspose.gridweb/gridpivottable)-elementet på det angivna indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar storleken på enumeratorn |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort PivotTable på det angivna indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


Lägger till en ny PivotTable-cache i en PivotCaches-samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Källarbetsbladet. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Området i källarbetsbladet. |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Det nyss tillagda cache‑indexet.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


Lägger till en ny PivotTable-cache i en PivotCaches-samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| worksheetname | java.lang.String | Namnet på källarbetsbladet. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Området i källarbetsbladet. |
| destRow | int | Raden för cellen i det övre vänstra hörnet av PivotTable-rapportens destinationsområde. |
| destCol | int | Kolumnen för cellen i det övre vänstra hörnet av PivotTable-rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Det nyss tillagda cache‑indexet.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


Lägger till en ny PivotTable-cache i en PivotCaches-samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| worksheetname | java.lang.String | Namnet på källarbetsbladet. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Området i källarbetsbladet. |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Det nyss tillagda cache‑indexet.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


Lägger till en ny PivotTable-cache i en PivotCaches-samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| sourceData | java.lang.String | Data‑cellområdet för den nya PivotTable. Exempel: Sheet1!A1:C8 |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av PivotTable‑rapportens destinationsområde. |
| tableName | java.lang.String | Namnet på den nya PivotTable‑rapporten. |

**Returns:**
int – Det nyss tillagda cache‑indexet.
### clear() {#clear--}
```
public void clear()
```


Rensar alla PivotTables.

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
### get(int index) {#get-int-}
```
public GridPivotTable get(int index)
```


Hämtar [GridPivotTable](../../com.aspose.gridweb/gridpivottable)-elementet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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


Hämtar storleken på enumeratorn

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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Tar bort PivotTable på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för elementet. |

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

