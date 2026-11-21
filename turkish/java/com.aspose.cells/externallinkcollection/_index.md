---
title: "ExternalLinkCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir çalışma kitabındaki harici bağlantılar koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/externallinkcollection/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Iterable
```
public class ExternalLinkCollection implements Iterable
```

Bir çalışma kitabındaki harici bağlantılar koleksiyonunu temsil eder.

**Example**

```
         //Open a file with external links
         Workbook workbook = new Workbook("book1.xls");
 
         //Change external link data source
         workbook.getWorksheets().getExternalLinks().get(0).setDataSource("d:\\link.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int directoryType, String fileName, String[] sheetNames)](#add-int-java.lang.String-java.lang.String---) | Bir dış bağlantı ekle. |
| [add(String fileName, String[] sheetNames)](#add-java.lang.String-java.lang.String---) | Bir dış bağlantı ekler. |
| [clear()](#clear--) | Tüm dış bağlantıları kaldırır. |
| [clear(boolean updateReferencesAsLocal)](#clear-boolean-) | Tüm dış bağlantıları kaldırır. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen dizindeki [ExternalLink](../../com.aspose.cells/externallink) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Koleksiyonda gerçekte bulunan öğe sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [iterator()](#iterator--) | Bu koleksiyon içinde yineleme yapan bir enumerator al. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dış bağlantıyı çalışma kitabından kaldırır. |
| [removeAt(int index, boolean updateReferencesAsLocal)](#removeAt-int-boolean-) | Belirtilen dış bağlantıyı çalışma kitabından kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int directoryType, String fileName, String[] sheetNames) {#add-int-java.lang.String-java.lang.String---}
```
public int add(int directoryType, String fileName, String[] sheetNames)
```


Bir dış bağlantı ekle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| directoryType | int | [DirectoryType](../../com.aspose.cells/directorytype). Dosya adının dizin türü. |
| fileName | java.lang.String | dosya adı. |
| sheetNames | java.lang.String[] | Harici dosyanın tüm sayfa adları. |

**Returns:**
int - Bu listedeki harici adın konumu.
### add(String fileName, String[] sheetNames) {#add-java.lang.String-java.lang.String---}
```
public int add(String fileName, String[] sheetNames)
```


Bir dış bağlantı ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| fileName | java.lang.String | Harici dosya adı. |
| sheetNames | java.lang.String[] | Harici dosyanın tüm sayfa adları. |

**Returns:**
int - Bu listedeki harici adın konumu.
### clear() {#clear--}
```
public void clear()
```


Tüm dış bağlantıları kaldırır.

**Remarks**

Harici bağlantılar kaldırıldığında, onlara başvuran tüm formüller de geçersiz referanslar olduğu için kaldırılacaktır.

### clear(boolean updateReferencesAsLocal) {#clear-boolean-}
```
public void clear(boolean updateReferencesAsLocal)
```


Tüm dış bağlantıları kaldırır.

**Remarks**

Referansların güncellenmesi gerekiyorsa, formüllerdeki harici bağlantı referansları mümkün olduğunda geçerli çalışma kitabına değiştirilecektir. Örneğin, bir hücrenin orijinal formülü "='externalsource.xlam'!customfunction()" ise, harici bağlantılar kaldırıldıktan sonra formül "=customfunction()" olur; Orijinal formül "='[externalsource.xlam]Sheet1'!$A$1" olduğunda, geçerli çalışma kitabında "Sheet1" adlı bir sayfa olup olmadığına göre: eğer varsa, formül "=Sheet1!$A$1" olur; yoksa, formül "=\#REF!$A$1" olur.

Referansların güncellenmesi gerekmiyorsa, harici bağlantılara referans içeren tüm formüller de geçersiz oldukları için kaldırılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| updateReferencesAsLocal | boolean | Formüllerdeki harici bağlantıların tüm referanslarının geçerli çalışma kitabına güncellenip güncellenmeyeceği. |

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
public ExternalLink get(int index)
```


Belirtilen dizindeki [ExternalLink](../../com.aspose.cells/externallink) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[ExternalLink](../../com.aspose.cells/externallink) - The element at the specified index.
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


Koleksiyonda gerçekte bulunan öğe sayısını alır.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### iterator() {#iterator--}
```
public Iterator iterator()
```


Bu koleksiyon içinde yineleme yapan bir enumerator al.

**Returns:**
java.util.Iterator -
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


Belirtilen dış bağlantıyı çalışma kitabından kaldırır.

**Remarks**

Harici bağlantı kaldırıldığında, ona başvuran tüm formüller de geçersiz referanslar olduğu için kaldırılacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak harici bağlantının dizini. |

### removeAt(int index, boolean updateReferencesAsLocal) {#removeAt-int-boolean-}
```
public void removeAt(int index, boolean updateReferencesAsLocal)
```


Belirtilen dış bağlantıyı çalışma kitabından kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak harici bağlantının dizini. |
| updateReferencesAsLocal | boolean | Verilen harici bağlantının tüm referanslarının geçerli çalışma kitabına güncellenip güncellenmeyeceği. Bu parametre hakkında daha fazla ayrıntı için [clear(boolean)](../../com.aspose.cells/externallinkcollection\#clear-boolean-) adresine bakın. |

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

