---
title: "TextBoxCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/textboxcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class TextBoxCollection extends CollectionBase
```

Bir [TextBox](../../com.aspose.cells/textbox) nesneleri koleksiyonunu kapsüller.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         //get collection object
         TextBoxCollection textBoxCollection = workbook.getWorksheets().get(0).getTextBoxes();
         //add a textbox
         textBoxCollection.add(1, 1, 50, 100);
         for(TextBox tbox : (Iterable<TextBox>) textBoxCollection)
         {
             //do what you want
         }
 
         //do your business
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(int topRow, int leftColumn, int height, int width)](#add-int-int-int-int-) | Koleksiyona bir metin kutusu ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | Tüm metin kutularını temizle. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [TextBox](../../com.aspose.cells/textbox) öğesini alır. |
| [get(String name)](#get-java.lang.String-) | İsme göre [TextBox](../../com.aspose.cells/textbox) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Dosyadan bir metin kutusunu kaldır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(int topRow, int leftColumn, int height, int width) {#add-int-int-int-int-}
```
public int add(int topRow, int leftColumn, int height, int width)
```


Koleksiyona bir metin kutusu ekler.

**Example**

```
         //add a TextBox
         int index2 = textBoxCollection.add(1, 1, 50, 100);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| üstSatır | int | Üst sol satır indeksi. |
| leftColumn | int | Üst sol sütun indeksi. |
| yükseklik | int | Metin kutusunun yüksekliği, piksel biriminde. |
| genişlik | int | Metin kutusunun genişliği, piksel biriminde. |

**Returns:**
int - [TextBox](../../com.aspose.cells/textbox) nesne indeksi.
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


Tüm metin kutularını temizle.

**Example**

```
         //clear all textbox
         textBoxCollection.clear();
```

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
public TextBox get(int index)
```


Belirtilen indeksteki [TextBox](../../com.aspose.cells/textbox) öğesini alır.

**Example**

```
         int index = textBoxCollection.getCount() - 1;
         TextBox txb = textBoxCollection.get(index);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - The element at the specified index.
### get(String name) {#get-java.lang.String-}
```
public TextBox get(String name)
```


İsme göre [TextBox](../../com.aspose.cells/textbox) öğesini alır.

**Example**

```
         String txtboxName = "textbox 1"; 
         TextBox txb2 = textBoxCollection.get(txtboxName);
         if(txb2 != null)
         {
             //do what you want
         }
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Metin kutusunun adı. |

**Returns:**
[TextBox](../../com.aspose.cells/textbox) - 
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


Dosyadan bir metin kutusunu kaldır.

**Example**

```
         int index3 = textBoxCollection.getCount() - 1;
         textBoxCollection.removeAt(index3);
```

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Metin kutusu indeksi. |

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

