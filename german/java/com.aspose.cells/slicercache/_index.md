---
title: "SlicerCache"
second_title: "Aspose.Cells for Java API-Referenz"
description: "Stellt die zusammenfassende Beschreibung des Slicer-Cache dar"
type: docs
url: /de/java/com.aspose.cells/slicercache/
---

**Inheritance:**
java.lang.Object
```
public class SlicerCache
```

Stellt die zusammenfassende Beschreibung des Slicer-Cache dar

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
## Methoden

| Methode | Beschreibung |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCrossFilterType()](#getCrossFilterType--) | Gibt an, wie Elemente ohne Daten im Slicer angezeigt werden. |
| [getList()](#getList--) | Gibt an, ob der mit dem angegebenen slicer cache verbundene slicer auf einer Non-OLAP-Datenquelle basiert. |
| [getName()](#getName--) | Gibt den Namen des slicer cache zurück. |
| [getSlicerCacheItems()](#getSlicerCacheItems--) | Gibt eine SlicerCacheItem collection zurück, die die Sammlung aller Elemente im slicer cache enthält. |
| [getSourceName()](#getSourceName--) | Gibt den Namen dieses slicer cache zurück. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCrossFilterType(int value)](#setCrossFilterType-int-) | Gibt an, wie Elemente ohne Daten im Slicer angezeigt werden. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


Gibt an, wie Elemente ohne Daten im Slicer angezeigt werden.

Siehe [SlicerCacheCrossFilterType](../../com.aspose.cells/slicercachecrossfiltertype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Slicer.getShowTypeOfItemsWithNoData()](../../com.aspose.cells/slicer\#getShowTypeOfItemsWithNoData--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Returns:**
int
### getList() {#getList--}
```
public boolean getList()
```


Gibt an, ob der mit dem angegebenen slicer cache verbundene slicer auf einer Non-OLAP-Datenquelle basiert.

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


Gibt den Namen des slicer cache zurück.

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


Gibt eine SlicerCacheItem‑Sammlung zurück, die die Sammlung aller Elemente im Slicer‑Cache enthält. Nur lesbar.

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


Gibt den Namen dieses slicer cache zurück.

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


Gibt an, wie Elemente ohne Daten im Slicer angezeigt werden.

Siehe [SlicerCacheCrossFilterType](../../com.aspose.cells/slicercachecrossfiltertype).

**Remarks**

HINWEIS: Dieses Mitglied ist jetzt veraltet. Verwenden Sie stattdessen die [Slicer.getShowTypeOfItemsWithNoData()](../../com.aspose.cells/slicer\#getShowTypeOfItemsWithNoData--) Eigenschaft. Diese Eigenschaft wird 12 Monate später, seit Januar 2026, entfernt. Aspose entschuldigt sich für etwaige Unannehmlichkeiten, die Sie möglicherweise erfahren haben.

**Parameters:**
| Parameter | Typ | Beschreibung |
| --- | --- | --- |
| Wert | int |  |

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

