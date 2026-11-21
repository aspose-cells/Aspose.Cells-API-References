---
title: "PivotFilterCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar en samling av alla PivotFilters."
type: docs
url: /sv/java/com.aspose.cells/pivotfiltercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class PivotFilterCollection extends CollectionBase
```

Representerar en samling av alla PivotFilters.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(int fieldIndex, int type)](#add-int-int-) | Lägger till ett PivotFilter-objekt till den specifika typen. |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)](#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-) | Filtrerar efter datuminställning för rad- eller kolumnpivotfält. |
| [addLabelFilter(int baseFieldIndex, int type, String label1, String label2)](#addLabelFilter-int-int-java.lang.String-java.lang.String-) | Filtrerar efter rubriker för rad- eller kolumnpivotfält. |
| [addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)](#addTop10Filter-int-int-int-boolean-int-) | Filtrerar efter värden för datapivotfält. |
| [addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)](#addValueFilter-int-int-int-double-double-) | Filtrerar efter värden för datapivotfält. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [clearFilter(int fieldIndex)](#clearFilter-int-) | Rensa PivotFilter från det specifika PivotField. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar pivotfilter-objektet vid det specifika indexet. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort objektet på det angivna indexet. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int fieldIndex, int type) {#add-int-int-}
```
public int add(int fieldIndex, int type)
```


Lägger till ett PivotFilter-objekt till den specifika typen.

**Remarks**

OBS: Denna metod är nu föråldrad. Använd istället metoderna PivotFilterCollection.AddValueFilter(),AddTop10Filter(),AddLabelFilter() och AddDateFilter(). Denna metod kommer att tas bort 12 månader senare sedan november 2024. Aspose ber om ursäkt för eventuella besvär du kan ha upplevt.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | PivotField-indexet |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). PivotFilter-typen |

**Returns:**
int - indexet för PivotFilter-objektet i denna PivotFilterCollection.
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


Lägger till ett objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Objektet som ska läggas till i CollectionBase-instansen. |

**Returns:**
int - Positionen där det nya elementet infördes.
### addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2) {#addDateFilter-int-int-com.aspose.cells.DateTime-com.aspose.cells.DateTime-}
```
public PivotFilter addDateFilter(int baseFieldIndex, int type, DateTime dateTime1, DateTime dateTime2)
```


Filtrerar efter datuminställning för rad- eller kolumnpivotfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseFieldIndex | int | Indexet för fältet i källan. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Typen av filtreringsdata. |
| dateTime1 | [DateTime](../../com.aspose.cells/datetime) | Datumetiketten för filtervillkoret |
| dateTime2 | [DateTime](../../com.aspose.cells/datetime) | Den övre gränsens datumetikett för mellanfiltervillkoret |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addLabelFilter(int baseFieldIndex, int type, String label1, String label2) {#addLabelFilter-int-int-java.lang.String-java.lang.String-}
```
public PivotFilter addLabelFilter(int baseFieldIndex, int type, String label1, String label2)
```


Filtrerar efter rubriker för rad- eller kolumnpivotfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseFieldIndex | int | Indexet för fältet i källan. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Typen av filtreringsdata. |
| label1 | java.lang.String | Etiketten för filtervillkoret |
| label2 | java.lang.String | Den övre gränsens etikett för mellanfiltervillkoret |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount) {#addTop10Filter-int-int-int-boolean-int-}
```
public PivotFilter addTop10Filter(int baseFieldIndex, int valueFieldIndex, int type, boolean isTop, int itemCount)
```


Filtrerar efter värden för datapivotfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseFieldIndex | int | Indexet för fältet i källan. |
| valueFieldIndex | int | Index för datafältet i dataområdet. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Typ av filtreringsdata. Kan endast vara Count, Sum och Percent. |
| isTop | boolean | Indikerar om filtret är från toppen eller botten. |
| itemCount | int | Antalet objekt. |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2) {#addValueFilter-int-int-int-double-double-}
```
public PivotFilter addValueFilter(int baseFieldIndex, int valueFieldIndex, int type, double value1, double value2)
```


Filtrerar efter värden för datapivotfält.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| baseFieldIndex | int | Indexet för fältet i källan. |
| valueFieldIndex | int | Index för värdefältet i värdeområdet. |
| type | int | [PivotFilterType](../../com.aspose.cells/pivotfiltertype). Typen av filtreringsdata. |
| value1 | double | Värdet för filtervillkoret. |
| value2 | double | Det övre gränsvärdet för mellanfiltervillkoret. |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
### clear() {#clear--}
```
public void clear()
```


Tar bort alla objekt från CollectionBase-instansen.

### clearFilter(int fieldIndex) {#clearFilter-int-}
```
public void clearFilter(int fieldIndex)
```


Rensa PivotFilter från det specifika PivotField.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| fieldIndex | int | PivotField-indexet |

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Returnerar om instansen innehåller detta objekt

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | testobjekt |

**Returns:**
boolean - Om instansen innehåller detta objekt
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
public PivotFilter get(int index)
```


Hämtar pivotfilter-objektet vid det specifika indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
[PivotFilter](../../com.aspose.cells/pivotfilter)
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


Hämtar antalet element som finns i CollectionBase-instansen.

**Returns:**
int - Antalet element som finns i CollectionBase-instansen.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object o) {#indexOf-java.lang.Object-}
```
public int indexOf(Object o)
```


Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| o | java.lang.Object | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |

**Returns:**
int - Indexet för värdet om det hittas i listan; annars -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


Returnerar en enumerator som itererar genom CollectionBase-instansen.

**Returns:**
java.util.Iterator - En iterator för CollectionBase-instansen.
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


Tar bort objektet på det angivna indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Det nollbaserade indexet för objektet som ska tas bort. |

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

