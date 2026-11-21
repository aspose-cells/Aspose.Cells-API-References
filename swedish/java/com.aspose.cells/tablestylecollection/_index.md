---
title: "TableStyleCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Representerar alla anpassade tabellstilar."
type: docs
url: /sv/java/com.aspose.cells/tablestylecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TableStyleCollection extends CollectionBase
```

Representerar alla anpassade tabellstilar.
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [addPivotTableStyle(String name)](#addPivotTableStyle-java.lang.String-) | Lägger till en anpassad pivottabellstil. |
| [addTableStyle(String name)](#addTableStyle-java.lang.String-) | Lägger till en anpassad tabellstil. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar tabellstilen med indexet. |
| [get(String name)](#get-java.lang.String-) | Hämtar tabellstilen med namn. |
| [getBuiltinTableStyle(int type)](#getBuiltinTableStyle-int-) | Hämtar den inbyggda tabellstilen |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [getDefaultPivotStyleName()](#getDefaultPivotStyleName--) | Hämtar standardstilens namn för pivottabellen. |
| [getDefaultTableStyleName()](#getDefaultTableStyleName--) | Hämtar standardstilens namn för tabellen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Tar bort objektet på det angivna indexet. |
| [setDefaultPivotStyleName(String value)](#setDefaultPivotStyleName-java.lang.String-) | Ställer in standardstilens namn för pivottabellen. |
| [setDefaultTableStyleName(String value)](#setDefaultTableStyleName-java.lang.String-) | Ställer in standardstilens namn för tabellen. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### addPivotTableStyle(String name) {#addPivotTableStyle-java.lang.String-}
```
public int addPivotTableStyle(String name)
```


Lägger till en anpassad pivottabellstil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Pivottabellens stilnamn. |

**Returns:**
int - Indexet för pivottabellens stil.
### addTableStyle(String name) {#addTableStyle-java.lang.String-}
```
public int addTableStyle(String name)
```


Lägger till en anpassad tabellstil.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Tabellstilens namn. |

**Returns:**
int - Indexet för tabellstilen.
### clear() {#clear--}
```
public void clear()
```


Tar bort alla objekt från CollectionBase-instansen.

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
public TableStyle get(int index)
```


Hämtar tabellstilen med indexet.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen för tabellstilen i listan. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### get(String name) {#get-java.lang.String-}
```
public TableStyle get(String name)
```


Hämtar tabellstilen med namn.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String | Tabellstilens namn. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - The table style object.
### getBuiltinTableStyle(int type) {#getBuiltinTableStyle-int-}
```
public TableStyle getBuiltinTableStyle(int type)
```


Hämtar den inbyggda tabellstilen

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| type | int | [TableStyleType](../../com.aspose.cells/tablestyletype). Den inbyggda tabellstilstypen. |

**Returns:**
[TableStyle](../../com.aspose.cells/tablestyle) - 
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
### getDefaultPivotStyleName() {#getDefaultPivotStyleName--}
```
public String getDefaultPivotStyleName()
```


Hämtar standardstilens namn för pivottabellen.

**Returns:**
java.lang.String
### getDefaultTableStyleName() {#getDefaultTableStyleName--}
```
public String getDefaultTableStyleName()
```


Hämtar standardstilens namn för tabellen.

**Returns:**
java.lang.String
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

### setDefaultPivotStyleName(String value) {#setDefaultPivotStyleName-java.lang.String-}
```
public void setDefaultPivotStyleName(String value)
```


Ställer in standardstilens namn för pivottabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

### setDefaultTableStyleName(String value) {#setDefaultTableStyleName-java.lang.String-}
```
public void setDefaultTableStyleName(String value)
```


Ställer in standardstilens namn för tabellen.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | java.lang.String |  |

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

