---
title: "DocumentPropertyCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "  ve  koleksiyonları için temel sınıf."
type: docs
url: /tr/java/com.aspose.cells/documentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public abstract class DocumentPropertyCollection extends CollectionBase
```

Temel sınıf, [BuiltInDocumentPropertyCollection](../../com.aspose.cells/builtindocumentpropertycollection) ve [CustomDocumentPropertyCollection](../../com.aspose.cells/customdocumentpropertycollection) koleksiyonları için.

**Example**

```
         //Instantiate a Workbook object by calling its empty constructor
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         DocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
 
         //Accessng a custom document property by using the property index
         DocumentProperty customProperty1 = customProperties.get(3);
 
         //Accessng a custom document property by using the property name
         DocumentProperty customProperty2 = customProperties.get("Owner");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [contains(String name)](#contains-java.lang.String-) | Belirtilen ada sahip bir özellik koleksiyonda mevcutsa true döndürür. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | İndeks ile bir [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesi döndürür. |
| [get(String name)](#get-java.lang.String-) | Özelliğin adıyla bir [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesi döndürür. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [indexOf(String name)](#indexOf-java.lang.String-) | Adına göre bir özelliğin indeksini alır. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(String name)](#remove-java.lang.String-) | Belirtilen ada sahip bir özelliği koleksiyondan kaldırır. |
| [removeAt(int index)](#removeAt-int-) | Belirtilen indeksteki bir özelliği kaldırır. |
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
### clear() {#clear--}
```
public void clear()
```


CollectionBase örneğinden tüm nesneleri kaldırır.

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
### contains(String name) {#contains-java.lang.String-}
```
public boolean contains(String name)
```


Belirtilen ada sahip bir özellik koleksiyonda mevcutsa true döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin büyük/küçük harfe duyarsız adı. |

**Returns:**
boolean - Özellik koleksiyonda mevcutsa true; aksi takdirde false.
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
public DocumentProperty get(int index)
```


İndeks ile bir [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesi döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| index | int | Alınacak [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesinin sıfır tabanlı indeksi. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
### get(String name) {#get-java.lang.String-}
```
public DocumentProperty get(String name)
```


Özelliğin adıyla bir [DocumentProperty](../../com.aspose.cells/documentproperty) nesnesi döndürür.

**Remarks**

Belirtilen ada sahip bir özellik bulunamazsa null döndürür.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Alınacak özelliğin büyük/küçük harfe duyarsız adı. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty)
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
### indexOf(String name) {#indexOf-java.lang.String-}
```
public int indexOf(String name)
```


Adına göre bir özelliğin indeksini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin büyük/küçük harfe duyarsız adı. |

**Returns:**
int - Sıfır tabanlı indeks. Bulunamazsa negatif değer.
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




### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Belirtilen ada sahip bir özelliği koleksiyondan kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin büyük/küçük harfe duyarsız adı. |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen indeksteki bir özelliği kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Sıfır tabanlı indeks. |

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

