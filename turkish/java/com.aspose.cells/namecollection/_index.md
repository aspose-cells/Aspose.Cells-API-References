---
title: "NameCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Elektronik tabloda bulunan tüm nesnelerin bir koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/namecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class NameCollection extends CollectionBase
```

Elektronik tabloda bulunan tüm [Name](../../com.aspose.cells/name) nesnelerinin bir koleksiyonunu temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String text)](#add-java.lang.String-) | Yeni bir ad tanımlar. |
| [clear()](#clear--) | Formüller ve veri kaynağı tarafından başvurulmayan tüm tanımlı adları kaldır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int type, int sheetIndex)](#filter-int-int-) | Kapsama göre tüm tanımlı adları al. |
| [get(int index)](#get-int-) | Belirtilen indeksteki [Name](../../com.aspose.cells/name) öğesini al. |
| [get(String text)](#get-java.lang.String-) | Belirtilen ada sahip [Name](../../com.aspose.cells/name) öğesini al. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String text)](#remove-java.lang.String-) | Adı kaldır. |
| [remove(String[] names)](#remove-java.lang.String---) | Adların bir dizisini kaldır. |
| [removeAt(int index)](#removeAt-int-) | Belirli indeksteki adı kaldır. |
| [removeDuplicateNames()](#removeDuplicateNames--) | Yinelenen tanımlı adları kaldır. |
| [sort()](#sort--) | Tanımlı adları sıralar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### add(String text) {#add-java.lang.String-}
```
public int add(String text)
```


Yeni bir ad tanımlar.

**Remarks**

Ad boşluk içeremez ve hücre referansı gibi görünemez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Ad olarak kullanılacak metin. |

**Returns:**
int - [Name](../../com.aspose.cells/name) nesne indeksi.
### clear() {#clear--}
```
public void clear()
```


Formüller ve veri kaynağı tarafından başvurulmayan tüm tanımlı adları kaldır. Tanımlı ada başvuruluyorsa, yalnızca Name.ReferTo'yu null olarak ayarlar ve onları gizleriz.

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
### filter(int type, int sheetIndex) {#filter-int-int-}
```
public Name[] filter(int type, int sheetIndex)
```


Kapsama göre tüm tanımlı adları al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [NameScopeType](../../com.aspose.cells/namescopetype). Kapsam türü. |
| sheetIndex | int | Sayfa indeksi. Yalnızca kapsam türü [NameScopeType.WORKSHEET](../../com.aspose.cells/namescopetype\#WORKSHEET) olduğunda etkili olur. |

**Returns:**
com.aspose.cells.Name[] -
### get(int index) {#get-int-}
```
public Name get(int index)
```


Belirtilen indeksteki [Name](../../com.aspose.cells/name) öğesini al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element at the specified index.
### get(String text) {#get-java.lang.String-}
```
public Name get(String text)
```


Belirtilen ada sahip [Name](../../com.aspose.cells/name) öğesini al.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Ad metni. |

**Returns:**
[Name](../../com.aspose.cells/name) - The element with the specified name.
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




### remove(String text) {#remove-java.lang.String-}
```
public void remove(String text)
```


Adı kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| metin | java.lang.String | Ad metni. |

### remove(String[] names) {#remove-java.lang.String---}
```
public void remove(String[] names)
```


Adların bir dizisini kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| adlar | java.lang.String[] | İsimlerin metni. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirli indeksteki adı kaldır.

**Remarks**

Lütfen yöntemi çağırmadan önce adın diğer formüller tarafından referans edilmediğinden emin olun. Ve eğer ad referans ediliyorsa, Name.RefersTo özelliğini null olarak ayarlamak daha iyidir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak Name'in dizini. |

### removeDuplicateNames() {#removeDuplicateNames--}
```
public void removeDuplicateNames()
```


Yinelenen tanımlı adları kaldır.

### sort() {#sort--}
```
public void sort()
```


Tanımlı adları sıralar.

**Remarks**

Excel dosyasında çok sayıda adlandırılmış aralık oluşturursanız, lütfen bu yöntemi tüm adlandırılmış aralıklar oluşturulduktan ve kaydetmeden önce çağırın.

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

