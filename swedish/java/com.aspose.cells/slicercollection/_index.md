---
title: "SlicerCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Anger samlingen av alla Slicer-objekt på det angivna kalkylbladet."
type: docs
url: /sv/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

Anger samlingen av alla Slicer-objekt på det angivna kalkylbladet.

**Example**

```
         Workbook book = new Workbook();
         Worksheet sheet = book.getWorksheets().get(0);
         Cells cells = sheet.getCells();
         cells.get(0, 0).setValue("fruit");
         cells.get(1, 0).setValue("grape");
         cells.get(2, 0).setValue("blueberry");
         cells.get(3, 0).setValue("kiwi");
         cells.get(4, 0).setValue("cherry");
         cells.get(5, 0).setValue("grape");
         cells.get(6, 0).setValue("blueberry");
         cells.get(7, 0).setValue("kiwi");
         cells.get(8, 0).setValue("cherry");
 
         cells.get(0, 1).setValue("year");
         cells.get(1, 1).setValue(2020);
         cells.get(2, 1).setValue(2020);
         cells.get(3, 1).setValue(2020);
         cells.get(4, 1).setValue(2020);
         cells.get(5, 1).setValue(2021);
         cells.get(6, 1).setValue(2021);
         cells.get(7, 1).setValue(2021);
         cells.get(8, 1).setValue(2021);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
         cells.get(5, 2).setValue(90);
         cells.get(6, 2).setValue(100);
         cells.get(7, 2).setValue(110);
         cells.get(8, 2).setValue(120);
 
         PivotTableCollection pivots = sheet.getPivotTables();
 
         PivotTable pivot = pivots.add("=Sheet1!A1:C9", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
 
         //do your business
 
         book.save("out.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | Lägg till en ny slicer som använder ListObjet som datakälla |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | Lägg till en ny slicer som använder ListObjet som datakälla |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | Lägg till en ny slicer som använder ListObjet som datakälla |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Lägg till en ny slicer som använder PivotTable som datakälla |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Lägg till en ny slicer som använder PivotTable som datakälla |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Lägg till en ny slicer som använder PivotTable som datakälla |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Lägg till en ny slicer som använder PivotTable som datakälla |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Lägg till en ny slicer som använder PivotTable som datakälla |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Lägg till en ny slicer som använder PivotTable som datakälla |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [clear()](#clear--) | Rensa alla slicers. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar slicern efter index. |
| [get(String name)](#get-java.lang.String-) | Hämtar slicern efter slicerns namn. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Hämtar antalet element som finns i CollectionBase-instansen. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | Bestämmer indexet för ett specifikt objekt i CollectionBase-instansen. |
| [iterator()](#iterator--) | Returnerar en enumerator som itererar genom CollectionBase-instansen. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | Ta bort den angivna slicern |
| [removeAt(int index)](#removeAt-int-) | Raderar slicern på det angivna indexet |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


Lägg till en ny slicer som använder ListObjet som datakälla

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject-objekt |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | ListColumn i ListObject.ListColumns |
| rad | int | Radindex för cellen i det övre vänstra hörnet av slicer-området. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av slicer-området. |

**Returns:**
int - Det nya tillagda slicer-indexet
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


Lägg till en ny slicer som använder ListObjet som datakälla

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject-objekt |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | ListColumn i ListObject.ListColumns |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av slicer-området. |

**Returns:**
int - Det nya tillagda slicer-indexet
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


Lägg till en ny slicer som använder ListObjet som datakälla

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject-objekt |
| index | int | Indexet för ListColumn i ListObject.ListColumns |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av slicer-området. |

**Returns:**
int - Det nya tillagda slicer-indexet
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Lägg till en ny slicer som använder PivotTable som datakälla

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| rad | int | Radindex för cellen i det övre vänstra hörnet av slicer-området. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av slicer-området. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda slicer-indexet
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Lägg till en ny slicer som använder PivotTable som datakälla

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| rad | int | Radindex för cellen i det övre vänstra hörnet av slicer-området. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av slicer-området. |
| baseFieldIndex | int | Indexet för PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda slicer-indexet
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Lägg till en ny slicer som använder PivotTable som datakälla

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| rad | int | Radindex för cellen i det övre vänstra hörnet av slicer-området. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av slicer-området. |
| baseFieldName | java.lang.String | Namnet på PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda slicer-indexet
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Lägg till en ny slicer som använder PivotTable som datakälla

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av slicer-området. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda slicer-indexet
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Lägg till en ny slicer som använder PivotTable som datakälla

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av slicer-området. |
| baseFieldIndex | int | Indexet för PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda slicer-indexet
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Lägg till en ny slicer som använder PivotTable som datakälla

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| destCellName | java.lang.String | Cellen i det övre vänstra hörnet av slicer-området. |
| baseFieldName | java.lang.String | Namnet på PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda slicer-indexet
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
### clear() {#clear--}
```
public void clear()
```


Rensa alla slicers.

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
public Slicer get(int index)
```


Hämtar slicern efter index.

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


Hämtar slicern efter slicerns namn.

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
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




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


Ta bort den angivna slicern

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | Slicer-objektet |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Raderar slicern på det angivna indexet

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int | Positionsindex i Slicer-samlingen |

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

