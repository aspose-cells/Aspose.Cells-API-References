---
title: "GridPivotTableCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.gridweb/gridpivottablecollection/
---

**Inheritance:**
java.lang.Object
```
public class GridPivotTableCollection
```

[GridPivotTable](../../com.aspose.gridweb/gridpivottable) nesnelerinden oluşan bir koleksiyonu kapsüller.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)](#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler. |
| [add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-) | PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler. |
| [add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)](#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-) | PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler. |
| [add(String sourceData, String destCellName, String tableName)](#add-java.lang.String-java.lang.String-java.lang.String-) | PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler. |
| [clear()](#clear--) | Tüm PivotTable'ları temizler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [GridPivotTable](../../com.aspose.gridweb/gridpivottable) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Yineleyicinin boyutunu alır |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen indeksteki PivotTable'ı kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName) {#add-com.aspose.gridweb.GridWorksheet-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(GridWorksheet sourceSheet, GridCellArea sourceArea, String destCellName, String tableName)
```


PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | Kaynak çalışma sayfası. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Kaynak çalışma sayfasındaki alan. |
| destCellName | java.lang.String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Yeni eklenen önbellek indeksi.
### add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-int-int-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, int destRow, int destCol, String tableName)
```


PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| worksheetname | java.lang.String | Kaynak çalışma sayfasının adı. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Kaynak çalışma sayfasındaki alan. |
| destRow | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin satırı. |
| destCol | int | PivotTable raporunun hedef aralığının sol üst köşesindeki hücrenin sütunu. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Yeni eklenen önbellek indeksi.
### add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName) {#add-java.lang.String-com.aspose.gridweb.GridCellArea-java.lang.String-java.lang.String-}
```
public int add(String worksheetname, GridCellArea sourceArea, String destCellName, String tableName)
```


PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| worksheetname | java.lang.String | Kaynak çalışma sayfasının adı. |
| sourceArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Kaynak çalışma sayfasındaki alan. |
| destCellName | java.lang.String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Yeni eklenen önbellek indeksi.
### add(String sourceData, String destCellName, String tableName) {#add-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String sourceData, String destCellName, String tableName)
```


PivotCaches koleksiyonuna yeni bir PivotTable önbelleği ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sourceData | java.lang.String | Yeni PivotTable için veri hücre aralığı. Örnek: Sheet1!A1:C8 |
| destCellName | java.lang.String | PivotTable raporunun hedef aralığının sol üst köşesindeki hücre. |
| tableName | java.lang.String | Yeni PivotTable raporunun adı. |

**Returns:**
int - Yeni eklenen önbellek indeksi.
### clear() {#clear--}
```
public void clear()
```


Tüm PivotTable'ları temizler.

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
public GridPivotTable get(int index)
```


Belirtilen indeksteki [GridPivotTable](../../com.aspose.gridweb/gridpivottable) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[GridPivotTable](../../com.aspose.gridweb/gridpivottable) - The element at the specified index.
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


Yineleyicinin boyutunu alır

**Returns:**
int
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen indeksteki PivotTable'ı kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

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

