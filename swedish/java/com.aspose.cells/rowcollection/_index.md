---
title: "RowCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Samlar objekten som representerar de enskilda raderna i ett kalkylblad."
type: docs
url: /sv/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

Samlar [Row](../../com.aspose.cells/row)-objekten som representerar de enskilda raderna i ett kalkylblad.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [clear()](#clear--) | Rensa alla rader och celler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Hämtar ett [Row](../../com.aspose.cells/row)-objekt med angivet radindex. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet rader i den här samlingen. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Hämtar radobjektet efter positionen i listan. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Hämtar en enumerator som itererar rader genom den här samlingen |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Hämtar en enumerator som itererar rader genom den här samlingen |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Ta bort radobjektet på det angivna indexet (positionen) i denna samling. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Rensa alla rader och celler.

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
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


Hämtar ett [Row](../../com.aspose.cells/row)-objekt med angivet radindex. Row-objektet för det angivna radindexet kommer att instansieras om det inte redan finns.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| rowIndex | int |  |

**Returns:**
[Row](../../com.aspose.cells/row)
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


Hämtar antalet rader i den här samlingen.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


Hämtar radobjektet efter positionen i listan.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionen. |

**Returns:**
[Row](../../com.aspose.cells/row) - The Row object at given position.
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


Hämtar en enumerator som itererar rader genom den här samlingen

**Example**

```
         Workbook workbook = new Workbook("template.xlsx");
         	Cells cells = workbook.getWorksheets().get(0).getCells();
 
         	Iterator en = cells.getRows().iterator();
         	while (en.hasNext())
         	{
         	    Row row = (Row)en.next();
         	    System.out.println(row.getIndex() + ": " + row.getHeight());
         	}
```

**Returns:**
java.util.Iterator - Radräknaren som kommer att gå igenom alla befintliga rader i denna samling.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Hämtar en enumerator som itererar rader genom den här samlingen

**Remarks**

Om radsamlingen kommer att modifieras (genom operationer som kan orsaka att en ny Row instansieras eller en befintlig Row tas bort) under traverseringen med räknaren, bör en synkroniserad räknare användas i stället för en normal räknare så att traverseringen kan fortsätta från positionen precis efter den som har traverserats av den senaste MoveNext(). Dock, förutom fördelen att inget element hoppar över eller traverseras flera gånger, är nackdelen med den synkroniserade räknaren att prestandan blir något försämrad jämfört med den normala räknaren.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| omvänd | boolean | om rader ska enumereras i omvänd ordning |
| synk | boolean | om den returnerade räknaren ska kontrollera ändringar i radsamlingen och hålla sig synkroniserad med den. |

**Returns:**
java.util.Iterator - Radräknaren som kommer att gå igenom alla befintliga rader i denna samling.
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


Ta bort radobjektet på det angivna indexet (positionen) i denna samling.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | nollbaserat index (position, inte [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)) för det befintliga radobjektet i denna samling. |

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

