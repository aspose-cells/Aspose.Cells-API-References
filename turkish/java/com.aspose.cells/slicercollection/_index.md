---
title: "SlicerCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Belirtilen çalışma sayfasındaki tüm Slicer nesnelerinin koleksiyonunu belirtir."
type: docs
url: /tr/java/com.aspose.cells/slicercollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class SlicerCollection extends CollectionBase
```

Belirtilen çalışma sayfasındaki tüm Slicer nesnelerinin koleksiyonunu belirtir.

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
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(ListObject table, ListColumn listColumn, int row, int column)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-) | Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle |
| [add(ListObject table, ListColumn listColumn, String destCellName)](#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-) | Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle |
| [add(ListObject table, int index, String destCellName)](#add-com.aspose.cells.ListObject-int-java.lang.String-) | Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle |
| [add(PivotTable pivot, int row, int column, PivotField baseField)](#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-) | Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle |
| [add(PivotTable pivot, int row, int column, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-int-int-int-) | Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle |
| [add(PivotTable pivot, int row, int column, String baseFieldName)](#add-com.aspose.cells.PivotTable-int-int-java.lang.String-) | Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle |
| [add(PivotTable pivot, String destCellName, PivotField baseField)](#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-) | Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle |
| [add(PivotTable pivot, String destCellName, int baseFieldIndex)](#add-com.aspose.cells.PivotTable-java.lang.String-int-) | Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle |
| [add(PivotTable pivot, String destCellName, String baseFieldName)](#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-) | Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | Tüm Slicer'ları temizle. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Slicer'ı indeksine göre alır. |
| [get(String name)](#get-java.lang.String-) | Slicer'ı adına göre alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Slicer slicer)](#remove-com.aspose.cells.Slicer-) | Belirtilen Slicer'ı kaldır |
| [removeAt(int index)](#removeAt-int-) | Belirtilen indeksteki Slicer'ı siler |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(ListObject table, ListColumn listColumn, int row, int column) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-int-int-}
```
public int add(ListObject table, ListColumn listColumn, int row, int column)
```


Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject nesnesi |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | ListObject.ListColumns içindeki ListColumn |
| satır | int | Slicer aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | Slicer aralığının sol üst köşesindeki hücrenin sütun indeksi. |

**Returns:**
int - Yeni eklenen Slicer indeksi
### add(ListObject table, ListColumn listColumn, String destCellName) {#add-com.aspose.cells.ListObject-com.aspose.cells.ListColumn-java.lang.String-}
```
public int add(ListObject table, ListColumn listColumn, String destCellName)
```


Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject nesnesi |
| listColumn | [ListColumn](../../com.aspose.cells/listcolumn) | ListObject.ListColumns içindeki ListColumn |
| destCellName | java.lang.String | Slicer aralığının sol üst köşesindeki hücre. |

**Returns:**
int - Yeni eklenen Slicer indeksi
### add(ListObject table, int index, String destCellName) {#add-com.aspose.cells.ListObject-int-java.lang.String-}
```
public int add(ListObject table, int index, String destCellName)
```


Veri kaynağı olarak ListObjet kullanan yeni bir Slicer ekle

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| table | [ListObject](../../com.aspose.cells/listobject) | ListObject nesnesi |
| dizin | int | ListObject.ListColumns içindeki ListColumn'un indeksi |
| destCellName | java.lang.String | Slicer aralığının sol üst köşesindeki hücre. |

**Returns:**
int - Yeni eklenen Slicer indeksi
### add(PivotTable pivot, int row, int column, PivotField baseField) {#add-com.aspose.cells.PivotTable-int-int-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, int row, int column, PivotField baseField)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle

**Example**

```
         slicers.add(pivot, 3, 12, pivot.getBaseFields().get(0));
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| satır | int | Slicer aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | Slicer aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotTable.BaseFields içindeki PivotField |

**Returns:**
int - Yeni eklenen Slicer indeksi
### add(PivotTable pivot, int row, int column, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-int-int-int-}
```
public int add(PivotTable pivot, int row, int column, int baseFieldIndex)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle

**Example**

```
         slicers.add(pivot, 20, 8, 0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| satır | int | Slicer aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | Slicer aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseFieldIndex | int | PivotTable.BaseFields içindeki PivotField'in indeksi |

**Returns:**
int - Yeni eklenen Slicer indeksi
### add(PivotTable pivot, int row, int column, String baseFieldName) {#add-com.aspose.cells.PivotTable-int-int-java.lang.String-}
```
public int add(PivotTable pivot, int row, int column, String baseFieldName)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle

**Example**

```
         slicers.add(pivot, 20, 12, "fruit");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| satır | int | Slicer aralığının sol üst köşesindeki hücrenin satır indeksi. |
| sütun | int | Slicer aralığının sol üst köşesindeki hücrenin sütun indeksi. |
| baseFieldName | java.lang.String | PivotTable.BaseFields içindeki PivotField'in adı |

**Returns:**
int - Yeni eklenen Slicer indeksi
### add(PivotTable pivot, String destCellName, PivotField baseField) {#add-com.aspose.cells.PivotTable-java.lang.String-com.aspose.cells.PivotField-}
```
public int add(PivotTable pivot, String destCellName, PivotField baseField)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle

**Example**

```
         slicers.add(pivot, "I3", pivot.getBaseFields().get(0));
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| destCellName | java.lang.String | Slicer aralığının sol üst köşesindeki hücre. |
| baseField | [PivotField](../../com.aspose.cells/pivotfield) | PivotTable.BaseFields içindeki PivotField |

**Returns:**
int - Yeni eklenen Slicer indeksi
### add(PivotTable pivot, String destCellName, int baseFieldIndex) {#add-com.aspose.cells.PivotTable-java.lang.String-int-}
```
public int add(PivotTable pivot, String destCellName, int baseFieldIndex)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle

**Example**

```
         slicers.add(pivot, "E20", 0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| destCellName | java.lang.String | Slicer aralığının sol üst köşesindeki hücre. |
| baseFieldIndex | int | PivotTable.BaseFields içindeki PivotField'in indeksi |

**Returns:**
int - Yeni eklenen Slicer indeksi
### add(PivotTable pivot, String destCellName, String baseFieldName) {#add-com.aspose.cells.PivotTable-java.lang.String-java.lang.String-}
```
public int add(PivotTable pivot, String destCellName, String baseFieldName)
```


Veri kaynağı olarak PivotTable kullanan yeni bir Slicer ekle

**Example**

```
         slicers.add(pivot, "E3", "fruit");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pivot | [PivotTable](../../com.aspose.cells/pivottable) | PivotTable nesnesi |
| destCellName | java.lang.String | Slicer aralığının sol üst köşesindeki hücre. |
| baseFieldName | java.lang.String | PivotTable.BaseFields içindeki PivotField'in adı |

**Returns:**
int - Yeni eklenen Slicer indeksi
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


Tüm Slicer'ları temizle.

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
public Slicer get(int index)
```


Slicer'ı indeksine göre alır.

**Example**

```
         Slicer slicerByIndex = slicers.get(0);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[Slicer](../../com.aspose.cells/slicer)
### get(String name) {#get-java.lang.String-}
```
public Slicer get(String name)
```


Slicer'ı adına göre alır.

**Example**

```
         Slicer slicerByName = slicers.get("fruit");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

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




### remove(Slicer slicer) {#remove-com.aspose.cells.Slicer-}
```
public void remove(Slicer slicer)
```


Belirtilen Slicer'ı kaldır

**Example**

```
         Slicer delSlicer = slicers.get(0);
         slicers.remove(delSlicer);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| slicer | [Slicer](../../com.aspose.cells/slicer) | Slicer nesnesi |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen indeksteki Slicer'ı siler

**Example**

```
         slicers.removeAt(1);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Slicer koleksiyonundaki konum indeksi |

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

