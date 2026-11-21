---
title: "GridValidationCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.gridweb/gridvalidationcollection/
---

**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```

Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnelerinden oluşan bir koleksiyonu kapsar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add()](#add--) | Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnesini koleksiyona ekleyin. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | Koleksiyona bir veri doğrulaması ekler. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnesini koleksiyona ekleyin. |
| [add(int row, int column)](#add-int-int-) | Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnesini koleksiyona ekleyin. Doğrulama belirtilen hücreye uygulanır. |
| [add(String cellname)](#add-java.lang.String-) | Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnesini koleksiyona ekleyin. Doğrulama belirtilen hücreye uygulanır. |
| [clear()](#clear--) | Tüm doğrulamaları temizler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki [GridValidation](../../com.aspose.gridweb/gridvalidation) öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Yineleyicinin boyutunu alır |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Verilen hücreye uygulanan doğrulamayı alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Belirtilen indeksteki doğrulamayı kaldırın. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```


Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnesini koleksiyona ekleyin.

**Remarks**

NOTE: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen GridValidationCollection.Add(row,col) yöntemini kullanın. Bu özellik, OCAK 2015 tarihinden itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```


Koleksiyona bir veri doğrulaması ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | Bu doğrulamayı içeren alan. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```


Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnesini koleksiyona ekleyin.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | Bir doğrulama nesnesi. |

**Returns:**
int - [GridValidation](../../com.aspose.gridweb/gridvalidation) nesne indeksi.
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```


Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnesini koleksiyona ekleyin. Doğrulama belirtilen hücreye uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```


Bir [GridValidation](../../com.aspose.gridweb/gridvalidation) nesnesini koleksiyona ekleyin. Doğrulama belirtilen hücreye uygulanır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellname | java.lang.String | hücrenin adı. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```


Tüm doğrulamaları temizler.

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
public GridValidation get(int index)
```


Belirtilen indeksteki [GridValidation](../../com.aspose.gridweb/gridvalidation) öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
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
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```


Verilen hücreye uygulanan doğrulamayı alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| satır | int | Satır indeksi. |
| sütun | int | Sütun indeksi. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
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




### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```


Belirtilen indeksteki doğrulamayı kaldırın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

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

