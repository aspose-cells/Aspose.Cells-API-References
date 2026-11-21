---
title: "VbaModuleCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Listeyi temsil eder"
type: docs
url: /tr/java/com.aspose.cells/vbamodulecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaModuleCollection extends CollectionBase
```

Listenin temsil ettiği [VbaModule](../../com.aspose.cells/vbamodule)

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject(); 
         // Add a new module.
         vbaProject.getModules().add(VbaModuleType.CLASS, "test");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Worksheet sheet)](#add-com.aspose.cells.Worksheet-) | Bir çalışma sayfası için modül ekler. |
| [add(int type, String name)](#add-int-java.lang.String-) | Modül ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [addDesignerStorage(String name, byte[] data)](#addDesignerStorage-java.lang.String-byte---) |  |
| [addUserForm(String name, String codes, byte[] designerStorage)](#addUserForm-java.lang.String-java.lang.String-byte---) | Kullanıcı formunu VBA Projesine ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Listedeki [VbaModule](../../com.aspose.cells/vbamodule) öğesini indeks ile alır. |
| [get(String name)](#get-java.lang.String-) | Listedeki [VbaModule](../../com.aspose.cells/vbamodule) öğesini ad ile alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [getDesignerStorage(String name)](#getDesignerStorage-java.lang.String-) | Tasarımcının verilerini temsil eder. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [remove(Worksheet sheet)](#remove-com.aspose.cells.Worksheet-) | Bir çalışma sayfası için modülü kaldırır. |
| [remove(String name)](#remove-java.lang.String-) | Modülü isimle kaldır. |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(Worksheet sheet) {#add-com.aspose.cells.Worksheet-}
```
public int add(Worksheet sheet)
```


Bir çalışma sayfası için modül ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Çalışma sayfası |

**Returns:**
int -
### add(int type, String name) {#add-int-java.lang.String-}
```
public int add(int type, String name)
```


Modül ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [VbaModuleType](../../com.aspose.cells/vbamoduletype). Modülün türü. |
| ad | java.lang.String | Modülün adı. |

**Returns:**
int -
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
### addDesignerStorage(String name, byte[] data) {#addDesignerStorage-java.lang.String-byte---}
```
public void addDesignerStorage(String name, byte[] data)
```




**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |
| veri | byte[] |  |

### addUserForm(String name, String codes, byte[] designerStorage) {#addUserForm-java.lang.String-java.lang.String-byte---}
```
public int addUserForm(String name, String codes, byte[] designerStorage)
```


Kullanıcı formunu VBA Projesine ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Kullanıcı formunun adı |
| kodlar | java.lang.String | Kullanıcı formu için kodlar |
| designerStorage | byte[] | kullanıcı formu ile ilgili tasarım ayarı |

**Returns:**
int -
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
public VbaModule get(int index)
```


Listedeki [VbaModule](../../com.aspose.cells/vbamodule) öğesini indeks ile alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | İndeks. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
### get(String name) {#get-java.lang.String-}
```
public VbaModule get(String name)
```


Listedeki [VbaModule](../../com.aspose.cells/vbamodule) öğesini ad ile alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Modülün adı. |

**Returns:**
[VbaModule](../../com.aspose.cells/vbamodule) - 
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
### getDesignerStorage(String name) {#getDesignerStorage-java.lang.String-}
```
public byte[] getDesignerStorage(String name)
```


Tasarımcının verilerini temsil eder.

**Remarks**

Bunları ayrıştırmayı desteklemiyoruz. Sadece kopyalama için.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

**Returns:**
byte[]
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




### remove(Worksheet sheet) {#remove-com.aspose.cells.Worksheet-}
```
public void remove(Worksheet sheet)
```


Bir çalışma sayfası için modülü kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sheet | [Worksheet](../../com.aspose.cells/worksheet) | Çalışma sayfası |

### remove(String name) {#remove-java.lang.String-}
```
public void remove(String name)
```


Modülü isimle kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String |  |

### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen dizindeki öğeyi kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak öğenin sıfır tabanlı dizini. |

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

