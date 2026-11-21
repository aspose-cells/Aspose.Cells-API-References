---
title: "VbaProjectReferenceCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "VBA projesinin tüm referanslarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/vbaprojectreferencecollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class VbaProjectReferenceCollection extends CollectionBase
```

VBA projesinin tüm referanslarını temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
          // Init VBA project.
         VbaProject vbaProject = workbook.getVbaProject();
         // Add vba project reference
         vbaProject.getReferences().addRegisteredReference("stdole", "*\\G{00020430-0000-0000-C000-000000000046}#2.0#0#C:\\Windows\\system32\\stdole2.tlb#OLE Automation");
         //Saving the Excel file
         workbook.save("book1.xlsm");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Bükülmüş bir tip kitaplığına ve onun genişletilmiş tip kitaplığına bir referans ekleyin. |
| [addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)](#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-) | Bükülmüş bir tip kitaplığına ve onun genişletilmiş tip kitaplığına bir referans ekleyin. |
| [addProjectReferernce(String name, String absoluteLibid, String relativeLibid)](#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-) | Harici bir VBA projesine bir referans ekler. |
| [addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)](#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-) | Harici bir VBA projesine bir referans ekler. |
| [addRegisteredReference(String name, String libid)](#addRegisteredReference-java.lang.String-java.lang.String-) | Bir Automation tip kitaplığına referans ekleyin. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [copy(VbaProjectReferenceCollection source)](#copy-com.aspose.cells.VbaProjectReferenceCollection-) | Diğer VBA projesinden referansları kopyalar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int i)](#get-int-) | Dizindeki referansı indeksle alın. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
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
### addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlReferernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlReferernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


Bükülmüş bir tip kitaplığına ve onun genişletilmiş tip kitaplığına bir referans ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Referansın adı. |
| libid | java.lang.String | Automation tip kitaplığının tanımlayıcısı. |
| twiddledlibid | java.lang.String | Bükülmüş tip kitaplığının tanımlayıcısı |
| extendedLibid | java.lang.String | Genişletilmiş tip kitaplığının tanımlayıcısı |

**Returns:**
int -
### addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid) {#addControlRefrernce-java.lang.String-java.lang.String-java.lang.String-java.lang.String-}
```
public int addControlRefrernce(String name, String libid, String twiddledlibid, String extendedLibid)
```


Bükülmüş bir tip kitaplığına ve onun genişletilmiş tip kitaplığına bir referans ekleyin.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen VbaProjectReferenceCollection.AddControlReferernce() yöntemini kullanın. Bu yöntem Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Referansın adı. |
| libid | java.lang.String | Automation tip kitaplığının tanımlayıcısı. |
| twiddledlibid | java.lang.String | Bükülmüş tip kitaplığının tanımlayıcısı |
| extendedLibid | java.lang.String | Genişletilmiş tip kitaplığının tanımlayıcısı |

**Returns:**
int -
### addProjectReferernce(String name, String absoluteLibid, String relativeLibid) {#addProjectReferernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectReferernce(String name, String absoluteLibid, String relativeLibid)
```


Harici bir VBA projesine bir referans ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Referansın adı. |
| absoluteLibid | java.lang.String | Mutlak bir yol içeren başvurulan VBA projesinin tanımlayıcısı. |
| relativeLibid | java.lang.String | Göreceli bir yol içeren başvurulan VBA projesinin tanımlayıcısı. |

**Returns:**
int -
### addProjectRefrernce(String name, String absoluteLibid, String relativeLibid) {#addProjectRefrernce-java.lang.String-java.lang.String-java.lang.String-}
```
public int addProjectRefrernce(String name, String absoluteLibid, String relativeLibid)
```


Harici bir VBA projesine bir referans ekler.

**Remarks**

NOT: Bu yöntem artık kullanımdan kaldırılmıştır. Bunun yerine, lütfen VbaProjectReferenceCollection.AddProjectReferernce() yöntemini kullanın. Bu yöntem Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Referansın adı. |
| absoluteLibid | java.lang.String | Mutlak bir yol içeren başvurulan VBA projesinin tanımlayıcısı. |
| relativeLibid | java.lang.String | Göreceli bir yol içeren başvurulan VBA projesinin tanımlayıcısı. |

**Returns:**
int -
### addRegisteredReference(String name, String libid) {#addRegisteredReference-java.lang.String-java.lang.String-}
```
public int addRegisteredReference(String name, String libid)
```


Bir Automation tip kitaplığına referans ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ad | java.lang.String | Referansın adı. |
| libid | java.lang.String | Automation tip kitaplığının tanımlayıcısı. |

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
### copy(VbaProjectReferenceCollection source) {#copy-com.aspose.cells.VbaProjectReferenceCollection-}
```
public void copy(VbaProjectReferenceCollection source)
```


Diğer VBA projesinden referansları kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| source | [VbaProjectReferenceCollection](../../com.aspose.cells/vbaprojectreferencecollection) | Kaynak referanslar. |

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
### get(int i) {#get-int-}
```
public VbaProjectReference get(int i)
```


Dizindeki referansı indeksle alın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| i | int | İndeks. |

**Returns:**
[VbaProjectReference](../../com.aspose.cells/vbaprojectreference) - 
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

