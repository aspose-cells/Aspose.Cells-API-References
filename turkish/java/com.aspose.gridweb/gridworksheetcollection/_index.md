---
title: "GridWorksheetCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.gridweb/gridworksheetcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class GridWorksheetCollection extends CollectionBase
```

[GridWorksheet](../../com.aspose.gridweb/gridworksheet) nesnelerinin bir koleksiyonunu kapsar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add()](#add--) | Koleksiyona bir çalışma sayfası ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String sheetName)](#add-java.lang.String-) | Koleksiyona bir çalışma sayfası ekler. |
| [addCopy(int sheetIndex)](#addCopy-int-) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar. |
| [addCopy(String sheetName)](#addCopy-java.lang.String-) | Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar. |
| [calculateFormula()](#calculateFormula--) | Formüllerin sonucunu hesaplar. |
| [clear()](#clear--) | Tüm çalışma sayfalarını temizler. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [GridWorksheet](../../com.aspose.gridweb/gridworksheet) öğesini alır. |
| [get(String sheetName)](#get-java.lang.String-) | Belirtilen adla [GridWorksheet](../../com.aspose.gridweb/gridworksheet) öğesini alır. |
| [getActiveSheetIndex()](#getActiveSheetIndex--) | Elektronik tablo açıldığında aktif çalışma sayfasının indeksini temsil eder. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Yineleyicinin boyutunu alır |
| [getDefaultFontName()](#getDefaultFontName--) | Denetimin varsayılan yazı tipi adını alır. |
| [getDefaultFontSize()](#getDefaultFontSize--) | ????????? |
| [getNames()](#getNames--) | Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır. |
| [getNumberDecimalSeparator()](#getNumberDecimalSeparator--) | Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [insert(int index, String sheetName)](#insert-int-java.lang.String-) | Bir çalışma sayfası ekleyin. |
| [iterator()](#iterator--) | Satırların yineleyicisini alır |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen indeksteki öğeyi kaldırır. |
| [removeAt(String name)](#removeAt-java.lang.String-) | Belirtilen isimdeki öğeyi kaldırır. |
| [setActiveSheetIndex(int value)](#setActiveSheetIndex-int-) | Elektronik tablo açıldığında aktif çalışma sayfasının indeksini temsil eder. |
| [setDefaultFontName(String value)](#setDefaultFontName-java.lang.String-) | Denetimin varsayılan yazı tipi adını ayarlar. |
| [setDefaultFontSize(FontUnit value)](#setDefaultFontSize-com.aspose.gridweb.FontUnit-) | ????????? |
| [setNumberDecimalSeparator(char value)](#setNumberDecimalSeparator-char-) | Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı ayarlar. |
| [setVisible(String sheetName, boolean isVisible)](#setVisible-java.lang.String-boolean-) | Sayfa için görünürlüğü ayarlar. |
| [swapSheet(int sheetIndex1, int sheetIndex2)](#swapSheet-int-int-) | İki sayfayı değiştirir. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Koleksiyona bir çalışma sayfası ekler.

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) nesnesi indeksi.
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
### add(String sheetName) {#add-java.lang.String-}
```
public GridWorksheet add(String sheetName)
```


Koleksiyona bir çalışma sayfası ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Çalışma sayfası adı |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) object.
### addCopy(int sheetIndex) {#addCopy-int-}
```
public int addCopy(int sheetIndex)
```


Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex | int | Kaynak çalışma sayfasının indeksi. |

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) nesnesi indeksi.
### addCopy(String sheetName) {#addCopy-java.lang.String-}
```
public int addCopy(String sheetName)
```


Koleksiyona bir çalışma sayfası ekler ve mevcut bir çalışma sayfasından verileri kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Kaynak çalışma sayfasının adı. |

**Returns:**
int - [GridWorksheet](../../com.aspose.gridweb/gridworksheet) nesnesi indeksi.
### calculateFormula() {#calculateFormula--}
```
public void calculateFormula()
```


Formüllerin sonucunu hesaplar.

### clear() {#clear--}
```
public void clear()
```


Tüm çalışma sayfalarını temizler.

**Remarks**

Bir çalışma kitabı bir çalışma sayfası içermelidir.

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
public GridWorksheet get(int index)
```


Belirtilen indeksteki [GridWorksheet](../../com.aspose.gridweb/gridworksheet) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The element at the specified index.
### get(String sheetName) {#get-java.lang.String-}
```
public GridWorksheet get(String sheetName)
```


Belirtilen adla [GridWorksheet](../../com.aspose.gridweb/gridworksheet) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Çalışma sayfasının adı. |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet) - The GridWorksheet with the name.
### getActiveSheetIndex() {#getActiveSheetIndex--}
```
public int getActiveSheetIndex()
```


Elektronik tablo açıldığında aktif çalışma sayfasının indeksini temsil eder.

**Remarks**

Sayfa indeksi sıfır tabanlıdır.

**Returns:**
int
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
### getDefaultFontName() {#getDefaultFontName--}
```
public String getDefaultFontName()
```


Denetimin varsayılan yazı tipi adını alır.

**Example**

```
             GridWeb GridWeb1=new GridWeb();
         		GridWeb1.setDefaultFontName("Arial");
```

**Returns:**
java.lang.String
### getDefaultFontSize() {#getDefaultFontSize--}
```
public FontUnit getDefaultFontSize()
```


?????????

**Returns:**
[FontUnit](../../com.aspose.gridweb/fontunit)
### getNames() {#getNames--}
```
public GridNameCollection getNames()
```


Elektronik tablodaki tüm Name nesnelerinin koleksiyonunu alır.

**Returns:**
[GridNameCollection](../../com.aspose.gridweb/gridnamecollection)
### getNumberDecimalSeparator() {#getNumberDecimalSeparator--}
```
public char getNumberDecimalSeparator()
```


Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı alır. Varsayılan, geçerli Bölgenin ondalık ayırıcısıdır.

**Returns:**
char
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
### insert(int index, String sheetName) {#insert-int-java.lang.String-}
```
public GridWorksheet insert(int index, String sheetName)
```


Bir çalışma sayfası ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Sayfa indeksi |
| sheetName | java.lang.String |  |

**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
### iterator() {#iterator--}
```
public Iterator iterator()
```


Satırların yineleyicisini alır

**Returns:**
java.util.Iterator - Satırların yineleyicisi
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


Belirtilen indeksteki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak öğenin indeks değeri. |

### removeAt(String name) {#removeAt-java.lang.String-}
```
public void removeAt(String name)
```


Belirtilen isimdeki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Kaldırılacak öğenin adı. |

### setActiveSheetIndex(int value) {#setActiveSheetIndex-int-}
```
public void setActiveSheetIndex(int value)
```


Elektronik tablo açıldığında aktif çalışma sayfasının indeksini temsil eder.

**Remarks**

Sayfa indeksi sıfır tabanlıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setDefaultFontName(String value) {#setDefaultFontName-java.lang.String-}
```
public void setDefaultFontName(String value)
```


Denetimin varsayılan yazı tipi adını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.String |  |

### setDefaultFontSize(FontUnit value) {#setDefaultFontSize-com.aspose.gridweb.FontUnit-}
```
public void setDefaultFontSize(FontUnit value)
```


?????????

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| value | [FontUnit](../../com.aspose.gridweb/fontunit) |  |

### setNumberDecimalSeparator(char value) {#setNumberDecimalSeparator-char-}
```
public void setNumberDecimalSeparator(char value)
```


Sayısal değerlerin biçimlendirilmesi/ayrıştırılması için ondalık ayırıcıyı ayarlar. Varsayılan, geçerli Bölgenin ondalık ayırıcısıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | char |  |

### setVisible(String sheetName, boolean isVisible) {#setVisible-java.lang.String-boolean-}
```
public void setVisible(String sheetName, boolean isVisible)
```


Sayfa için görünürlüğü ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetName | java.lang.String | Kaynak çalışma sayfasının adı. |
| isVisible | boolean | Çalışma sayfasının görünür olup olmadığı |

### swapSheet(int sheetIndex1, int sheetIndex2) {#swapSheet-int-int-}
```
public void swapSheet(int sheetIndex1, int sheetIndex2)
```


İki sayfayı değiştirir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheetIndex1 | int | İlk çalışma sayfası. |
| sheetIndex2 | int | İkinci çalışma sayfası. |

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

