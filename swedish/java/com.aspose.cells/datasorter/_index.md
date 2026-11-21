---
title: "DataSorter"
second_title: "Aspose.Cells för Java API-referens"
description: "Sammanfattande beskrivning för DataSorter."
type: docs
url: /sv/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

Sammanfattande beskrivning för DataSorter.

**Example**

```
         //Instantiate a new Workbook object.
         Workbook workbook = new Workbook("Book1.xls");
         //Get the workbook datasorter object.
         DataSorter sorter = workbook.getDataSorter();
         //Set the first order for datasorter object.
         sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
         //Define the first key.
         sorter.setKey1(0);
         //Set the second order for datasorter object.
         sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
         //Define the second key.
         sorter.setKey2(1);
         //Create a cells area (range).
         CellArea ca = new CellArea();
         //Specify the start row index.
         ca.StartRow = 0;
         //Specify the start column index.
         ca.StartColumn = 0;
         //Specify the last row index.
         ca.EndRow = 13;
         //Specify the last column index.
         ca.EndColumn = 1;
         //Sort data in the specified data range (A1:B14)
         sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
         //Save the excel file.
         workbook.save("outBook.xls");
```
## Metoder

| Metod | Beskrivning |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | Lägger till färgsorteringsnyckel. |
| [addKey(int key, int order)](#addKey-int-int-) | Lägger till sorterat kolumnindex och sorteringsordning. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista. |
| [clear()](#clear--) | Rensa alla inställningar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Hämtar om skiftlägeskänslig vid jämförelse av sträng. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | Representerar första sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...). |
| [getKey2()](#getKey2--) | Representerar andra sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...). |
| [getKey3()](#getKey3--) | Representerar tredje sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...). |
| [getKeys()](#getKeys--) | Hämtar nyckellistan för data sorter. |
| [getOrder1()](#getOrder1--) | Representerar sorteringsordning för den första nyckeln. |
| [getOrder2()](#getOrder2--) | Representerar sorteringsordning för den andra nyckeln. |
| [getOrder3()](#getOrder3--) | Representerar sorteringsordning för den tredje nyckeln. |
| [getSortAsNumber()](#getSortAsNumber--) | Indikerar om sortering av allt som ser ut som ett tal. |
| [getSortLeftToRight()](#getSortLeftToRight--) | Sant betyder att sorteringsorienteringen är från vänster till höger. |
| [hasHeaders()](#hasHeaders--) | Representerar om intervallet har rubriker. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Anger om jämförelsen av sträng är skiftlägeskänslig. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | Representerar om intervallet har rubriker. |
| [setKey1(int value)](#setKey1-int-) | Representerar första sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...). |
| [setKey2(int value)](#setKey2-int-) | Representerar andra sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...). |
| [setKey3(int value)](#setKey3-int-) | Representerar tredje sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...). |
| [setOrder1(int value)](#setOrder1-int-) | Representerar sorteringsordning för den första nyckeln. |
| [setOrder2(int value)](#setOrder2-int-) | Representerar sorteringsordning för den andra nyckeln. |
| [setOrder3(int value)](#setOrder3-int-) | Representerar sorteringsordning för den tredje nyckeln. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | Indikerar om sortering av allt som ser ut som ett tal. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | Sant betyder att sorteringsorienteringen är från vänster till höger. |
| [sort()](#sort--) | Sortera data i intervallet. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | Sortera data i området. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | Sorterar data i området. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


Lägger till färgsorteringsnyckel.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | int | Det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Den sorterade färgvärdestypen. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringsordningen. |
| color | [Color](../../com.aspose.cells/color) | Den anpassade sorteringsfärgen. |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


Lägger till sorterat kolumnindex och sorteringsordning.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | int | Det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringsordningen |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista.

**Remarks**

Om typen är SortOnType.CellColor eller SortOnType.FontColor, är customList en Color.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | int | Det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Den sorterade värdetypen. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringsordningen. |
| customList | java.lang.Object | Den anpassade sorteringslistan. |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | int | Det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringsordningen. |
| customList | java.lang.String | Den anpassade sorteringslistan. |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


Lägger till sorterat kolumnindex och sorteringsordning med anpassad sorteringslista.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| nyckel | int | Det sorterade kolumnindexet (absolut position, kolumn A är 0, B är 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sorteringsordningen. |
| customList | java.lang.String[] | Den anpassade sorteringslistan. |

### clear() {#clear--}
```
public void clear()
```


Rensa alla inställningar.

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Hämtar om skiftlägeskänslig vid jämförelse av sträng.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```


Representerar första sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...).

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


Representerar andra sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...).

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


Representerar tredje sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...).

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


Hämtar nyckellistan för data sorter.

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


Representerar sorteringsordning för den första nyckeln.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


Representerar sorteringsordning för den andra nyckeln.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


Representerar sorteringsordning för den tredje nyckeln.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


Indikerar om sortering av allt som ser ut som ett tal.

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True betyder att sorteringsorienteringen är från vänster till höger. False betyder att sorteringsorienteringen är från topp till botten. Standardvärdet är false.

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


Representerar om intervallet har rubriker.

**Returns:**
boolean
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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Anger om jämförelsen av sträng är skiftlägeskänslig.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


Representerar om intervallet har rubriker.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


Representerar första sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


Representerar andra sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


Representerar tredje sorterade kolumnindex(absolut position, kolumn A är 0, B är 1, ...).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


Representerar sorteringsordning för den första nyckeln.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


Representerar sorteringsordning för den andra nyckeln.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


Representerar sorteringsordning för den tredje nyckeln.

Se [SortOrder](../../com.aspose.cells/sortorder).

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


Indikerar om sortering av allt som ser ut som ett tal.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True betyder att sorteringsorienteringen är från vänster till höger. False betyder att sorteringsorienteringen är från topp till botten. Standardvärdet är false.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| värde | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


Sortera data i intervallet.

**Returns:**
int[] – de ursprungliga indexen (absolut position, till exempel kolumn A är 0, B är 1, ...) för de sorterade raderna/kolumnerna. Om inga rader/kolumner behöver flyttas av denna sorteringsoperation, returneras null.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


Sortera data i området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Cellerna innehåller dataområdet. |
| area | [CellArea](../../com.aspose.cells/cellarea) | Området som behövs för sortering |

**Returns:**
int[] – de ursprungliga indexen (absolut position, till exempel kolumn A är 0, B är 1, ...) för de sorterade raderna/kolumnerna. Om inga rader/kolumner behöver flyttas av denna sorteringsoperation, returneras null.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


Sorterar data i området.

**Parameters:**
| Parameter | Typ | Beskrivning |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Cellerna innehåller dataområdet. |
| startRad | int | Startraden för området. |
| startColumn | int | Startkolumnen för området. |
| slutRad | int | Slutraden för området. |
| endColumn | int | Slutkolumnen för området. |

**Returns:**
int[] – de ursprungliga indexen (absolut position, till exempel kolumn A är 0, B är 1, ...) för de sorterade raderna/kolumnerna. Om inga rader/kolumner behöver flyttas av denna sorteringsoperation, returneras null.
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

