---
title: "SlicerCache"
second_title: "Справочник API Aspose.Cells for Java"
description: "Представляет краткое описание кэша среза."
type: docs
url: /ru/java/com.aspose.cells/slicercache/
---

**Inheritance:**
java.lang.Object
```
public class SlicerCache
```

Представляет краткое описание кэша среза.

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
 
         //Add a PivotTable
         PivotTable pivot = pivots.add("=Sheet1!A1:C5", "A12");
         pivot.addFieldToArea(PivotFieldType.ROW, "fruit");
         pivot.addFieldToArea(PivotFieldType.COLUMN, "year");
         pivot.addFieldToArea(PivotFieldType.DATA, "amount");
 
         pivot.setPivotTableStyleType(PivotTableStyleType.PIVOT_TABLE_STYLE_MEDIUM_10);
 
         pivot.calculateData();
 
         SlicerCollection slicers = sheet.getSlicers();
         int slicerIndex = slicers.add(pivot, "E12", "fruit");
         Slicer slicer = slicers.get(slicerIndex);
         slicer.setStyleType(SlicerStyleType.SLICER_STYLE_LIGHT_2);
 
         //Get SlicerCache object of current slicer
         SlicerCache slicerCache = slicer.getSlicerCache();
 
         //do your business
 
         book.save("out.xlsx");
```
## Методы

| Метод | Описание |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCrossFilterType()](#getCrossFilterType--) | Указывает, как отображать элементы без данных в слайсере. |
| [getList()](#getList--) | Указывает, основан ли слайсер, связанный с указанным кэшем слайсера, на источнике данных Non-OLAP. |
| [getName()](#getName--) | Возвращает имя кэша слайсера. |
| [getSlicerCacheItems()](#getSlicerCacheItems--) | Возвращает коллекцию SlicerCacheItem, содержащую все элементы в кэше слайсера. |
| [getSourceName()](#getSourceName--) | Возвращает имя этого кэша слайсера. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCrossFilterType(int value)](#setCrossFilterType-int-) | Указывает, как отображать элементы без данных в слайсере. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Параметр | Тип | Описание |
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
### getCrossFilterType() {#getCrossFilterType--}
```
public int getCrossFilterType()
```


Указывает, как отображать элементы без данных в слайсере.

См. [SlicerCacheCrossFilterType](../../com.aspose.cells/slicercachecrossfiltertype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство [Slicer.getShowTypeOfItemsWithNoData()](../../com.aspose.cells/slicer\#getShowTypeOfItemsWithNoData--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Returns:**
int
### getList() {#getList--}
```
public boolean getList()
```


Указывает, основан ли слайсер, связанный с указанным кэшем слайсера, на источнике данных Non-OLAP.

**Example**

```
         System.out.println(slicerCache.getList());
```

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


Возвращает имя кэша слайсера.

**Example**

```
         //get the name of the slicer cache.
         System.out.println(slicerCache.getName());
```

**Returns:**
java.lang.String
### getSlicerCacheItems() {#getSlicerCacheItems--}
```
public SlicerCacheItemCollection getSlicerCacheItems()
```


Возвращает коллекцию SlicerCacheItem, содержащую все элементы в кэше среза. Только для чтения.

**Example**

```
         //get SlicerCacheItem collection that contains the collection of all items in the slicer cache.
         SlicerCacheItemCollection slicerCacheItems = slicerCache.getSlicerCacheItems();
         System.out.println(slicerCacheItems.getCount());
```

**Returns:**
[SlicerCacheItemCollection](../../com.aspose.cells/slicercacheitemcollection)
### getSourceName() {#getSourceName--}
```
public String getSourceName()
```


Возвращает имя этого кэша слайсера.

**Example**

```
         //get the name of this slicer cache.
         System.out.println(slicerCache.getSourceName());
```

**Returns:**
java.lang.String
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




### setCrossFilterType(int value) {#setCrossFilterType-int-}
```
public void setCrossFilterType(int value)
```


Указывает, как отображать элементы без данных в слайсере.

См. [SlicerCacheCrossFilterType](../../com.aspose.cells/slicercachecrossfiltertype).

**Remarks**

ПРИМЕЧАНИЕ: Этот член теперь устарел. Вместо этого, пожалуйста, используйте свойство [Slicer.getShowTypeOfItemsWithNoData()](../../com.aspose.cells/slicer\#getShowTypeOfItemsWithNoData--). Это свойство будет удалено через 12 месяцев, начиная с января 2026 года. Aspose приносит извинения за любые неудобства, которые вы могли испытать.

**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| значение | int |  |

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
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Параметр | Тип | Описание |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

