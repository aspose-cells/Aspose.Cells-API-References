---
title: "PivotPageFields"
second_title: "Aspose.Cells for Java API Referansı"
description: "Pivot tablo veri kaynağı konsolidasyon aralıkları ise pivot sayfa öğelerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/pivotpagefields/
---

**Inheritance:**
java.lang.Object
```
public class PivotPageFields
```

Pivot tablo veri kaynağı konsolidasyon aralıkları ise pivot sayfa öğelerini temsil eder. En fazla 4 öğe içerebilir.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [PivotPageFields()](#PivotPageFields--) | Pivot sayfa alanı öğelerini temsil eder. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addIdentify(int rangeIndex, int[] pageItemIndex)](#addIdentify-int-int---) | Her sayfa alanındaki hangi öğe etiketinin veri aralığını tanımlamak için kullanılacağını ayarlar. |
| [addPageField(String[] pageItems)](#addPageField-java.lang.String---) | Bir sayfa alanı ekler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPageFieldCount()](#getPageFieldCount--) | Sayfa alanlarının sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotPageFields() {#PivotPageFields--}
```
public PivotPageFields()
```


Pivot sayfa alanı öğelerini temsil eder.

### addIdentify(int rangeIndex, int[] pageItemIndex) {#addIdentify-int-int---}
```
public void addIdentify(int rangeIndex, int[] pageItemIndex)
```


Her sayfa alanındaki hangi öğe etiketinin veri aralığını tanımlamak için kullanılacağını ayarlar. pageItemIndex.Length, PageFieldCount değerine eşit olmalıdır; bu yüzden önce sayfa alanını ekleyiniz.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rangeIndex | int | Konsolidasyon veri aralığı indeksi. |
| pageItemIndex | int[] | Her sayfa alanındaki sayfa öğesi indeksi. pageItemIndex[2] = 1, bu aralığı tanımlamak için üçüncü alandaki ikinci öğe anlamına gelir. pageItemIndex[1] = -1, ikinci alanda bu aralığı tanımlamak için öğe olmadığını ve MS'nin ikinci alanda bu aralığı tanımlamak için otomatik olarak "boş" bir öğe oluşturacağını gösterir. |

### addPageField(String[] pageItems) {#addPageField-java.lang.String---}
```
public void addPageField(String[] pageItems)
```


Bir sayfa alanı ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| pageItems | java.lang.String[] | Sayfa alanı öğe etiketi |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPageFieldCount() {#getPageFieldCount--}
```
public int getPageFieldCount()
```


Sayfa alanlarının sayısını alır.

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

