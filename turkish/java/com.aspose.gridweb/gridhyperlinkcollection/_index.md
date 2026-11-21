---
title: "GridHyperlinkCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.gridweb/gridhyperlinkcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlinkCollection
```

Bir koleksiyon [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) nesnelerini kapsar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler. |
| [add(String cellName, String address)](#add-java.lang.String-java.lang.String-) | Belirtilen bir hücreye bir köprü ekler. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler. |
| [clear()](#clear--) | Tüm bağlantıları temizler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen dizindeki [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Yineleyicinin boyutunu alır |
| [getHyperlink(GridCell cell)](#getHyperlink-com.aspose.gridweb.GridCell-) | Hücrenin Köprü nesnesini alır. |
| [getHyperlink(int row, int column)](#getHyperlink-int-int-) | Hücrenin Köprü nesnesini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(GridCellArea area)](#remove-com.aspose.gridweb.GridCellArea-) | Belirtilen alandaki köprüyü kaldır. |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki köprüyü kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bağlantı aralığının ilk satırı. |
| firstColumn | int | Bağlantı aralığının ilk sütunu. |
| totalRows | int | Bu bağlantı aralığındaki satır sayısı. |
| totalColumns | int | Bu bağlantı aralığındaki sütun sayısı. |
| adres | java.lang.String | Köprü adresi. |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) nesne indeksi.
### add(String cellName, int totalRows, int totalColumns, String address) {#add-java.lang.String-int-int-java.lang.String-}
```
public int add(String cellName, int totalRows, int totalColumns, String address)
```


Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |
| totalRows | int | Bu bağlantı aralığındaki satır sayısı. |
| totalColumns | int | Bu bağlantı aralığındaki sütun sayısı. |
| adres | java.lang.String | Köprü adresi. |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) nesne indeksi.
### add(String cellName, String address) {#add-java.lang.String-java.lang.String-}
```
public int add(String cellName, String address)
```


Belirtilen bir hücreye bir köprü ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellName | java.lang.String | Hücre adı. |
| adres | java.lang.String | Köprü adresi. |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) nesne indeksi.
### add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip) {#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)
```


Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startCellName | java.lang.String | Aralığın sol üst hücresi. |
| endCellName | java.lang.String | Aralığın sağ alt hücresi. |
| adres | java.lang.String | Köprü adresi. |
| textToDisplay | java.lang.String | Belirtilen bağlantı için görüntülenecek metin. |
| screenTip | java.lang.String | Belirtilen bağlantı için ekran ipucu metni. |

**Returns:**
int - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) nesne indeksi.
### clear() {#clear--}
```
public void clear()
```


Tüm bağlantıları temizler.

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
public GridHyperlink get(int index)
```


Belirtilen dizindeki [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - The element at the specified index.
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
### getHyperlink(GridCell cell) {#getHyperlink-com.aspose.gridweb.GridCell-}
```
public GridHyperlink getHyperlink(GridCell cell)
```


Hücrenin Köprü nesnesini alır. Hücrede Köprü yoksa, null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cell | [GridCell](../../com.aspose.gridweb/gridcell) | GridCell nesnesi. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
### getHyperlink(int row, int column) {#getHyperlink-int-int-}
```
public GridHyperlink getHyperlink(int row, int column)
```


Hücrenin Köprü nesnesini alır. Hücrede Köprü yoksa, null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Hücrenin satırı. |
| sütun | int | Hücrenin sütunu. |

**Returns:**
[GridHyperlink](../../com.aspose.gridweb/gridhyperlink) - [GridHyperlink](../../com.aspose.gridweb/gridhyperlink) the GridHyperlink object.
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




### remove(GridCellArea area) {#remove-com.aspose.gridweb.GridCellArea-}
```
public void remove(GridCellArea area)
```


Belirtilen alandaki köprüyü kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| area | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Bağlantıyı içeren alan. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen dizindeki köprüyü kaldır.

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

