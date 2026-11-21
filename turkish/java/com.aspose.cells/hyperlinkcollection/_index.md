---
title: "HyperlinkCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/hyperlinkcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class HyperlinkCollection extends CollectionBase
```

Bir [Hyperlink](../../com.aspose.cells/hyperlink) nesneleri koleksiyonunu kapsar.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Get Hyperlinks Collection
         HyperlinkCollection hyperlinks = worksheet.getHyperlinks();
 
         //Adding a hyperlink to a URL at "A1" cell
         hyperlinks.add("A1", 1, 1, "http://www.aspose.com");
 
         //Saving the Excel file
         workbook.save("book1.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)](#add-int-int-int-int-java.lang.String-) | Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String cellName, int totalRows, int totalColumns, String address)](#add-java.lang.String-int-int-java.lang.String-) | Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler. |
| [add(String startCellName, String endCellName, String address, String textToDisplay, String screenTip)](#add-java.lang.String-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler. |
| [clear()](#clear--) | Tüm bağlantıları temizler. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [Hyperlink](../../com.aspose.cells/hyperlink) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Bu koleksiyonda belirtilen indeksteki bağlantıyı kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address) {#add-int-int-int-int-java.lang.String-}
```
public int add(int firstRow, int firstColumn, int totalRows, int totalColumns, String address)
```


Belirtilen bir hücreye veya hücre aralığına bir bağlantı ekler.

**Example**

```
         //Instantiating a Workbook object
         Workbook excel = new Workbook();
         Worksheet worksheet = excel.getWorksheets().get(0);
         worksheet.getHyperlinks().add("A4", 1, 1, "http://www.aspose.com");
         worksheet.getHyperlinks().add("A5", 1, 1, "c:\\book1.xls");
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| firstRow | int | Bağlantı aralığının ilk satırı. |
| firstColumn | int | Bağlantı aralığının ilk sütunu. |
| totalRows | int | Bu bağlantı aralığındaki satır sayısı. |
| totalColumns | int | Bu bağlantı aralığındaki sütun sayısı. |
| adres | java.lang.String | Köprü adresi. |

**Returns:**
int - [Hyperlink](../../com.aspose.cells/hyperlink) nesne indeksi.
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
int - [Hyperlink](../../com.aspose.cells/hyperlink) nesne indeksi.
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
int - [Hyperlink](../../com.aspose.cells/hyperlink) nesne indeksi.
### clear() {#clear--}
```
public void clear()
```


Tüm bağlantıları temizler.

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
public Hyperlink get(int index)
```


Belirtilen indeksteki [Hyperlink](../../com.aspose.cells/hyperlink) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[Hyperlink](../../com.aspose.cells/hyperlink) - The element at the specified index.
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


Bu koleksiyonda belirtilen indeksteki bağlantıyı kaldır.

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

