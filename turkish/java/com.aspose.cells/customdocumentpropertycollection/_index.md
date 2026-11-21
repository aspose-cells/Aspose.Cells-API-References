---
title: "CustomDocumentPropertyCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Özel belge özelliklerinin bir koleksiyonu."
type: docs
url: /tr/java/com.aspose.cells/customdocumentpropertycollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase), [com.aspose.cells.DocumentPropertyCollection](../../com.aspose.cells/documentpropertycollection)
```
public class CustomDocumentPropertyCollection extends DocumentPropertyCollection
```

Özel belge özelliklerinin bir koleksiyonu.

**Remarks**

Her nesne, bir kapsayıcı belgenin özel bir özelliğini temsil eder.

**Example**

```
         //Instantiate a Workbook object
         Workbook workbook = new Workbook("book1.xls");
 
         //Retrieve a list of all custom document properties of the Excel file
         CustomDocumentPropertyCollection customProperties = workbook.getWorksheets().getCustomDocumentProperties();
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [add(String name, boolean value)](#add-java.lang.String-boolean-) | **PropertyType.Boolean** veri tipinde yeni bir özel belge özelliği oluşturur. |
| [add(String name, DateTime value)](#add-java.lang.String-com.aspose.cells.DateTime-) | **PropertyType.DateTime** veri tipinde yeni bir özel belge özelliği oluşturur. |
| [add(String name, double value)](#add-java.lang.String-double-) | Yeni bir **PropertyType.Float** veri tipinde özel belge özelliği oluşturur. |
| [add(String name, int value)](#add-java.lang.String-int-) | Yeni bir **PropertyType.Number** veri tipinde özel belge özelliği oluşturur. |
| [add(String name, String value)](#add-java.lang.String-java.lang.String-) | Yeni bir **PropertyType.String** veri tipinde özel belge özelliği oluşturur. |
| [addLinkToContent(String name, String source)](#addLinkToContent-java.lang.String-java.lang.String-) | İçeriğe bağlanan yeni bir özel belge özelliği oluşturur. |
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
| [updateLinkedPropertyValue()](#updateLinkedPropertyValue--) | İçeriğe bağlı tüm özel özelliklerin değerlerini günceller (bağlı aralığın hücre değerini kullanarak özel özelliğin değerini günceller). |
| [updateLinkedRange()](#updateLinkedRange--) | Özel özelliklere bağlı tüm aralıkları günceller (özel belge özelliğinin değerini kullanarak bağlı aralığın hücre değerini günceller). |
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
### add(String name, boolean value) {#add-java.lang.String-boolean-}
```
public DocumentProperty add(String name, boolean value)
```


**PropertyType.Boolean** veri tipinde yeni bir özel belge özelliği oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin adı. |
| değer | boolean | Özelliğin değeri. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, DateTime value) {#add-java.lang.String-com.aspose.cells.DateTime-}
```
public DocumentProperty add(String name, DateTime value)
```


**PropertyType.DateTime** veri tipinde yeni bir özel belge özelliği oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin adı. |
| value | [DateTime](../../com.aspose.cells/datetime) | Özelliğin değeri. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, double value) {#add-java.lang.String-double-}
```
public DocumentProperty add(String name, double value)
```


Yeni bir **PropertyType.Float** veri tipinde özel belge özelliği oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin adı. |
| değer | double | Özelliğin değeri. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, int value) {#add-java.lang.String-int-}
```
public DocumentProperty add(String name, int value)
```


Yeni bir **PropertyType.Number** veri tipinde özel belge özelliği oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin adı. |
| değer | int | Özelliğin değeri. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### add(String name, String value) {#add-java.lang.String-java.lang.String-}
```
public DocumentProperty add(String name, String value)
```


Yeni bir **PropertyType.String** veri tipinde özel belge özelliği oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin adı. |
| değer | java.lang.String | Özelliğin değeri. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
### addLinkToContent(String name, String source) {#addLinkToContent-java.lang.String-java.lang.String-}
```
public DocumentProperty addLinkToContent(String name, String source)
```


İçeriğe bağlanan yeni bir özel belge özelliği oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Özelliğin adı. |
| kaynak | java.lang.String | Özelliğin kaynağı. Adlandırılmış aralığın adı olmalıdır. |

**Returns:**
[DocumentProperty](../../com.aspose.cells/documentproperty) - The newly created property object.
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
### updateLinkedPropertyValue() {#updateLinkedPropertyValue--}
```
public void updateLinkedPropertyValue()
```


İçeriğe bağlı tüm özel özelliklerin değerlerini günceller (bağlı aralığın hücre değerini kullanarak özel özelliğin değerini günceller).

### updateLinkedRange() {#updateLinkedRange--}
```
public void updateLinkedRange()
```


Özel özelliklere bağlı tüm aralıkları günceller (özel belge özelliğinin değerini kullanarak bağlı aralığın hücre değerini günceller).

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

