---
title: "CustomCommandButtonCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "CustomCommandButton koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.gridweb/customcommandbuttoncollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.CollectionBase](../../com.aspose.gridweb/collectionbase)
```
public class CustomCommandButtonCollection extends CollectionBase
```

CustomCommandButton koleksiyonunu temsil eder.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         CustomCommandButton button = new CustomCommandButton();
         button.setCommand("MyCommand");
         button.setImageUrl("images/button1.gif");
         GridWeb1.getCustomCommandButtons().add(button);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object value)](#add-java.lang.Object-) | Koleksiyona özel bir komut düğmesi nesnesi ekleyin. |
| [clear()](#clear--) | Koleksiyonu temizler. |
| [contains(Object value)](#contains-java.lang.Object-) | Özel komut düğmesi nesnesinin koleksiyonda olup olmadığını gösterir. |
| [copyTo(Object[] array, int index)](#copyTo-java.lang.Object---int-) | Koleksiyonu bir diziye kopyalar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki özel komut düğmesi nesnesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Koleksiyonun sayısını alır. |
| [getSyncRoot()](#getSyncRoot--) | Yalnızca dahili kullanım için. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object value)](#indexOf-java.lang.Object-) | Düğmenin indeksini alır. |
| [insert(int index, Object value)](#insert-int-java.lang.Object-) | İndekste bir düğme ekler. |
| [isFixedSize()](#isFixedSize--) | Yalnızca dahili kullanım için. |
| [isReadOnly()](#isReadOnly--) | Yalnızca dahili kullanım için. |
| [isSynchronized()](#isSynchronized--) | Yalnızca dahili kullanım için. |
| [iterator()](#iterator--) | Koleksiyonun bir IEnumerator nesnesini alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Object value)](#remove-java.lang.Object-) | Özel komut düğmesi nesnesini kaldırır. |
| [removeAt(int index)](#removeAt-int-) | İndeksten kaldırır. |
| [set(int index, CustomCommandButton value)](#set-int-com.aspose.gridweb.CustomCommandButton-) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Object value) {#add-java.lang.Object-}
```
public int add(Object value)
```


Koleksiyona özel bir komut düğmesi nesnesi ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | Özel komut düğmesi nesnesi. |

**Returns:**
int - İndeks.
### clear() {#clear--}
```
public void clear()
```


Koleksiyonu temizler.

### contains(Object value) {#contains-java.lang.Object-}
```
public boolean contains(Object value)
```


Özel komut düğmesi nesnesinin koleksiyonda olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | Özel komut düğmesi nesnesinin koleksiyonda olup olmadığını gösterir. |

**Returns:**
boolean - Doğru veya yanlış.
### copyTo(Object[] array, int index) {#copyTo-java.lang.Object---int-}
```
public void copyTo(Object[] array, int index)
```


Koleksiyonu bir diziye kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizi | java.lang.Object[] | Dizi. |
| dizin | int | Dizinin başlangıç indeksi. |

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
public CustomCommandButton get(int index)
```


Belirtilen indeksteki özel komut düğmesi nesnesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |

**Returns:**
[CustomCommandButton](../../com.aspose.gridweb/customcommandbutton)
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


Koleksiyonun sayısını alır.

**Returns:**
int
### getSyncRoot() {#getSyncRoot--}
```
public Object getSyncRoot()
```


Yalnızca dahili kullanım için.

**Returns:**
java.lang.Object
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### indexOf(Object value) {#indexOf-java.lang.Object-}
```
public int indexOf(Object value)
```


Düğmenin indeksini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | Düğme nesnesi. |

**Returns:**
int - İndeks.
### insert(int index, Object value) {#insert-int-java.lang.Object-}
```
public void insert(int index, Object value)
```


İndekste bir düğme ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |
| değer | java.lang.Object | CustomCommandButton nesnesi. |

### isFixedSize() {#isFixedSize--}
```
public boolean isFixedSize()
```


Yalnızca dahili kullanım için.

**Returns:**
boolean
### isReadOnly() {#isReadOnly--}
```
public boolean isReadOnly()
```


Yalnızca dahili kullanım için.

**Returns:**
boolean
### isSynchronized() {#isSynchronized--}
```
public boolean isSynchronized()
```


Yalnızca dahili kullanım için.

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Koleksiyonun bir IEnumerator nesnesini alır.

**Returns:**
java.util.Iterator - IEnumerator nesnesi.
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### remove(Object value) {#remove-java.lang.Object-}
```
public void remove(Object value)
```


Özel komut düğmesi nesnesini kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | java.lang.Object | Özel komut düğmesi nesnesi. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


İndeksten kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

### set(int index, CustomCommandButton value) {#set-int-com.aspose.gridweb.CustomCommandButton-}
```
public void set(int index, CustomCommandButton value)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int |  |
| value | [CustomCommandButton](../../com.aspose.gridweb/customcommandbutton) |  |

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

