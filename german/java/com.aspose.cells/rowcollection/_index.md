---
title: "RowCollection"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Sammelt die Objekte, die die einzelnen Zeilen in einem Arbeitsblatt darstellen."
type: docs
url: /de/java/com.aspose.cells/rowcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class RowCollection implements Iterable
```

Sammelt die [Row](../../com.aspose.cells/row)-Objekte, die die einzelnen Zeilen in einem Arbeitsblatt darstellen.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the first worksheet
         Worksheet worksheet = workbook.getWorksheets().get(0);
          //Get first row
         Row row = worksheet.getCells().getRows().get(0);
```
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [clear()](#clear--) | Löscht alle Zeilen und Zellen. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int rowIndex)](#get-int-) | Ruft ein [Row](../../com.aspose.cells/row)-Objekt anhand des angegebenen Zeilenindex ab. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Ruft die Anzahl der Zeilen in dieser Sammlung ab. |
| [getRowByIndex(int index)](#getRowByIndex-int-) | Ruft das Zeilenobjekt anhand seiner Position in der Liste ab. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Ruft einen Enumerator ab, der Zeilen durch diese Sammlung iteriert |
| [iterator(boolean reversed, boolean sync)](#iterator-boolean-boolean-) | Ruft einen Enumerator ab, der Zeilen durch diese Sammlung iteriert |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Entfernt das Zeilenobjekt am angegebenen Index (Position) in dieser Sammlung. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### clear() {#clear--}
```
public void clear()
```


Löscht alle Zeilen und Zellen.

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int rowIndex) {#get-int-}
```
public Row get(int rowIndex)
```


Ruft ein [Row](../../com.aspose.cells/row)-Objekt anhand des angegebenen Zeilenindex ab. Das Row-Objekt des angegebenen Zeilenindex wird instanziiert, falls es vorher nicht existiert.

**Parameters:**
| Parameter | Typ | Beschreibung |
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


Ruft die Anzahl der Zeilen in dieser Sammlung ab.

**Returns:**
int
### getRowByIndex(int index) {#getRowByIndex-int-}
```
public Row getRowByIndex(int index)
```


Ruft das Zeilenobjekt anhand seiner Position in der Liste ab.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Index | int | Die Position. |

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


Ruft einen Enumerator ab, der Zeilen durch diese Sammlung iteriert

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
java.util.Iterator – Der Zeilenenumerator, der alle vorhandenen Zeilen in dieser Sammlung durchläuft.
### iterator(boolean reversed, boolean sync) {#iterator-boolean-boolean-}
```
public Iterator iterator(boolean reversed, boolean sync)
```


Ruft einen Enumerator ab, der Zeilen durch diese Sammlung iteriert

**Remarks**

Wenn die Zeilen­sammlung während der Durchquerung mit dem Enumerator geändert wird (durch Vorgänge, die dazu führen können, dass ein neues Row instanziiert oder ein vorhandenes Row entfernt wird), sollte ein synchronisierter Enumerator anstelle eines normalen Enumerators verwendet werden, damit die Durchquerung ab der Position fortgesetzt werden kann, die unmittelbar nach der zuletzt durch MoveNext() durchlaufenen liegt. Dabei besteht der Vorteil, dass kein Element übersprungen oder mehrfach durchlaufen wird; der Nachteil des synchronisierten Enumerators ist jedoch, dass die Leistung im Vergleich zu einem normalen Enumerator etwas reduziert wird.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| umgekehrt | boolean | ob Zeilen in umgekehrter Reihenfolge enumeriert werden |
| synchronisieren | boolean | ob der zurückgegebene Enumerator Änderungen der Zeilensammlung prüfen und mit ihr synchronisiert bleiben soll. |

**Returns:**
java.util.Iterator – Der Zeilenenumerator, der alle vorhandenen Zeilen in dieser Sammlung durchläuft.
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


Entfernt das Zeilenobjekt am angegebenen Index (Position) in dieser Sammlung.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| index | int | nullbasierter Index (Position, nicht [Row.getIndex()](../../com.aspose.cells/row\#getIndex--)) des vorhandenen Zeilenobjekts in dieser Sammlung. |

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
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

