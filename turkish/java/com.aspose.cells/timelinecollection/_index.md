---
title: "TimelineCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Çalışma sayfasındaki tüm nesnelerin koleksiyonunu belirtir."
type: docs
url: /tr/java/com.aspose.cells/timelinecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TimelineCollection extends CollectionBase
```

Çalışma sayfasındaki tüm [Timeline](../../com.aspose.cells/timeline) nesnelerinin koleksiyonunu belirtir. Excel 2013'ten beri desteklenmektedir.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Timeline'ı indeksine göre alır. |
| [get(String name)](#get-java.lang.String-) | Timeline'ı adına göre alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 20, 5, pivot.getBaseFields().get(1));
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| satır | int | Timeline aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | Timeline aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotTable.BaseFields içindeki PivotField |

**Returns:**
int - Yeni eklenen Timeline indeksi
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 15, 5, 1);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| satır | int | Timeline aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | Timeline aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseFieldIndex | int | PivotTable.BaseFields içindeki PivotField'in indeksi |

**Returns:**
int - Yeni eklenen Timeline indeksi
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, 10, 5, "date");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| satır | int | Timeline aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | Timeline aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseFieldName | java.lang.String | PivotTable.BaseFields içindeki PivotField'in adı |

**Returns:**
int - Yeni eklenen Timeline indeksi
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i10", pivot.getBaseFields().get(1));
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| destCellName | java.lang.String | Timeline aralığının sol üst köşesindeki hücrenin adı. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotTable.BaseFields içindeki PivotField |

**Returns:**
int - Yeni eklenen Timeline indeksi
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i5", 1);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| destCellName | java.lang.String | Timeline aralığının sol üst köşesindeki hücrenin adı. |
| baseFieldIndex | int | PivotTable.BaseFields içindeki PivotField'in indeksi |

**Returns:**
int - Yeni eklenen Timeline indeksi
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Timeline ekle

**Example**

```
         //Add a new Timeline using PivotTable as data source
         sheet.getTimelines().add(pivot, "i15", "date");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| destCellName | java.lang.String | Timeline aralığının sol üst köşesindeki hücrenin adı. |
| baseFieldName | java.lang.String | PivotTable.BaseFields içindeki PivotField'in adı |

**Returns:**
int - Yeni eklenen Timeline indeksi
### add(Object o) {#add-java.lang.Object-}
```
public int add(Object o)
```


CollectionBase örneğine bir öğe ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğine eklenecek Nesne. |

**Returns:**
int - Yeni elemanın eklendiği konum.
### clear() {#clear--}
```
public void clear()
```


CollectionBase örneğinden tüm nesneleri kaldırır.

### contains(Object o) {#contains-java.lang.Object-}
```
public boolean contains(Object o)
```


Örneğin bu nesneyi içerip içermediğini döndürür

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | test nesnesi |

**Returns:**
boolean - Örneğin bu nesneyi içerip içermediği
### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### get(int index) {#get-int-}
```
public Timeline get(int index)
```


Timeline'ı indeksine göre alır.

**Example**

```
         //Get the Timeline by index.
         Timeline objByIndex = sheet.getTimelines().get(0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[Timeline](../../com.aspose.cells/timeline)
### get(String name) {#get-java.lang.String-}
```
public Timeline get(String name)
```


Timeline'ı adına göre alır.

**Example**

```
         //Get the Timeline by Timeline's name.
         Timeline objByName = sheet.getTimelines().get("date");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

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


CollectionBase örneğinde bulunan eleman sayısını alır.

**Returns:**
int - CollectionBase örneğinde bulunan eleman sayısı.
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


CollectionBase örneğindeki belirli bir öğenin dizinini belirler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| o | java.lang.Object | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |

**Returns:**
int - Değer listede bulunursa dizini; aksi takdirde -1.
### iterator() {#iterator--}
```
public Iterator iterator()
```


CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür.

**Returns:**
java.util.Iterator - CollectionBase örneği için bir iterator.
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


Belirtilen dizindeki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak öğenin sıfır tabanlı dizini. |

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
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

