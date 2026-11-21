---
title: "TimelineCollection"
second_title: "Aspose.Cells för Java API-referens"
description: "Anger samlingen av alla objekt på kalkylbladet."
type: docs
url: /sv/java/com.aspose.cells/timelinecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TimelineCollection extends CollectionBase
```

Anger samlingen av alla [Timeline](../../com.aspose.cells/timeline) objekt på kalkylbladet. Det har stödts sedan Excel 2013.

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
 
         //Create date style
         Style dateStyle = new CellsFactory().createStyle();
         dateStyle.setCustom("m/d/yyyy");
         cells.get(0, 1).setValue("date");
         cells.get(1, 1).setValue(new DateTime(2021, 2, 5));
         cells.get(2, 1).setValue(new DateTime(2022, 3, 8));
         cells.get(3, 1).setValue(new DateTime(2023, 4, 10));
         cells.get(4, 1).setValue(new DateTime(2024, 5, 16));
         //Set date style
         cells.get(1, 1).setStyle(dateStyle);
         cells.get(2, 1).setStyle(dateStyle);
         cells.get(3, 1).setStyle(dateStyle);
         cells.get(4, 1).setStyle(dateStyle);
 
         cells.get(0, 2).setValue("amount");
         cells.get(1, 2).setValue(50);
         cells.get(2, 2).setValue(60);
         cells.get(3, 2).setValue(70);
         cells.get(4, 2).setValue(80);
 
         PivotTableCollection pivots = sheet.getPivotTables();
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
 
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "date");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         //do your business
 
         book.save("out.xlsx");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Lägg till en ny Timeline med PivotTable som datakälla |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Lägg till en ny Timeline med PivotTable som datakälla |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Lägg till en ny Timeline med PivotTable som datakälla |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Lägg till en ny Timeline med PivotTable som datakälla |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Lägg till en ny Timeline med PivotTable som datakälla |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Lägg till en ny Timeline med PivotTable som datakälla |
| [add(Object o)](#add-java.lang.Object-) | Lägger till ett objekt i CollectionBase-instansen. |
| [clear()](#clear--) | Tar bort alla objekt från CollectionBase-instansen. |
| [contains(Object o)](#contains-java.lang.Object-) | Returnerar om instansen innehåller detta objekt |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Hämtar Timeline efter index. |
| [get(String name)](#get-java.lang.String-) | Hämtar Timeline efter Timelines namn. |
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
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Lägg till en ny Timeline med PivotTable som datakälla

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 20, 5, pivot.getBaseFields().get(1));
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| rad | int | Radindex för cellen i det övre vänstra hörnet av Timeline-området. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av Timeline-området. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda Timeline-indexet
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Lägg till en ny Timeline med PivotTable som datakälla

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 15, 5, 1);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| rad | int | Radindex för cellen i det övre vänstra hörnet av Timeline-området. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av Timeline-området. |
| baseFieldIndex | int | Indexet för PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda Timeline-indexet
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Lägg till en ny Timeline med PivotTable som datakälla

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 10, 5, "date");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| rad | int | Radindex för cellen i det övre vänstra hörnet av Timeline-området. |
| kolumn | int | Kolumnindex för cellen i det övre vänstra hörnet av Timeline-området. |
| baseFieldName | java.lang.String | Namnet på PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda Timeline-indexet
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Lägg till en ny Timeline med PivotTable som datakälla

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i10", pivot.getBaseFields().get(1));
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| destCellName | java.lang.String | Cellnamnet i det övre vänstra hörnet av Timeline-området. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda Timeline-indexet
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Lägg till en ny Timeline med PivotTable som datakälla

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i5", 1);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| destCellName | java.lang.String | Cellnamnet i det övre vänstra hörnet av Timeline-området. |
| baseFieldIndex | int | Indexet för PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda Timeline-indexet
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Lägg till en ny Timeline med PivotTable som datakälla

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i15", "date");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable-objekt |
| destCellName | java.lang.String | Cellnamnet i det övre vänstra hörnet av Timeline-området. |
| baseFieldName | java.lang.String | Namnet på PivotField i PivotTable.BaseFields |

**Returns:**
int - Det nya tillagda Timeline-indexet
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
public Timeline get(int index)
```


Hämtar Timeline efter index.

**Example**

```
         //Get the Timeline by index.
         Timeline objByIndex = sheet.getTimelines().get(0);
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| index | int |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
### get(String name) {#get-java.lang.String-}
```
public Timeline get(String name)
```


Hämtar Timeline efter Timelines namn.

**Example**

```
         //Get the Timeline by Timeline's name.
         Timeline objByName = sheet.getTimelines().get("date");
```

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| name | java.lang.String |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
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

