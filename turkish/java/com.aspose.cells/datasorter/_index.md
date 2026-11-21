---
title: "DataSorter"
second_title: "Aspose.Cells for Java API Referansı"
description: "DataSorter için özet açıklama."
type: docs
url: /tr/java/com.aspose.cells/datasorter/
---

**Inheritance:**
java.lang.Object
```
public class DataSorter
```

DataSorter için özet açıklama.

**Example**

```
         //Instantiate a new Workbook object.
         Workbook workbook = new Workbook("Book1.xls");
         //Get the workbook datasorter object.
         DataSorter sorter = workbook.getDataSorter();
         //Set the first order for datasorter object.
         sorter.setOrder1(com.aspose.cells.SortOrder.DESCENDING);
         //Define the first key.
         sorter.setKey1(0);
         //Set the second order for datasorter object.
         sorter.setOrder2(com.aspose.cells.SortOrder.ASCENDING);
         //Define the second key.
         sorter.setKey2(1);
         //Create a cells area (range).
         CellArea ca = new CellArea();
         //Specify the start row index.
         ca.StartRow = 0;
         //Specify the start column index.
         ca.StartColumn = 0;
         //Specify the last row index.
         ca.EndRow = 13;
         //Specify the last column index.
         ca.EndColumn = 1;
         //Sort data in the specified data range (A1:B14)
         sorter.sort(workbook.getWorksheets().get(0).getCells(), ca);
         //Save the excel file.
         workbook.save("outBook.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [addColorKey(int key, int type, int order, Color color)](#addColorKey-int-int-int-com.aspose.cells.Color-) | Renk sıralama anahtarını ekler. |
| [addKey(int key, int order)](#addKey-int-int-) | Sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [addKey(int key, int type, int order, Object customList)](#addKey-int-int-int-java.lang.Object-) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [addKey(int key, int order, String customList)](#addKey-int-int-java.lang.String-) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [addKey(int key, int order, String[] customList)](#addKey-int-int-java.lang.String---) | Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler. |
| [clear()](#clear--) | Tüm ayarları temizle. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCaseSensitive()](#getCaseSensitive--) | Dize karşılaştırılırken büyük/küçük harfe duyarlı olup olmadığını alır. |
| [getClass()](#getClass--) |  |
| [getKey1()](#getKey1--) | İlk sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [getKey2()](#getKey2--) | İkinci sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [getKey3()](#getKey3--) | Üçüncü sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [getKeys()](#getKeys--) | Veri sıralayıcının anahtar listesini alır. |
| [getOrder1()](#getOrder1--) | İlk anahtarın sıralama düzenini temsil eder. |
| [getOrder2()](#getOrder2--) | İkinci anahtarın sıralama düzenini temsil eder. |
| [getOrder3()](#getOrder3--) | Üçüncü anahtarın sıralama düzenini temsil eder. |
| [getSortAsNumber()](#getSortAsNumber--) | Bir sayıya benzeyen şeylerin sıralanıp sıralanmayacağını gösterir. |
| [getSortLeftToRight()](#getSortLeftToRight--) | Doğru, sıralama yönünün soldan sağa olduğunu gösterir. |
| [hasHeaders()](#hasHeaders--) | Aralığın başlık içerip içermediğini temsil eder. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCaseSensitive(boolean value)](#setCaseSensitive-boolean-) | Dize karşılaştırılırken büyük/küçük harfe duyarlı olup olmadığını ayarlar. |
| [setHasHeaders(boolean value)](#setHasHeaders-boolean-) | Aralığın başlık içerip içermediğini temsil eder. |
| [setKey1(int value)](#setKey1-int-) | İlk sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [setKey2(int value)](#setKey2-int-) | İkinci sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [setKey3(int value)](#setKey3-int-) | Üçüncü sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...). |
| [setOrder1(int value)](#setOrder1-int-) | İlk anahtarın sıralama düzenini temsil eder. |
| [setOrder2(int value)](#setOrder2-int-) | İkinci anahtarın sıralama düzenini temsil eder. |
| [setOrder3(int value)](#setOrder3-int-) | Üçüncü anahtarın sıralama düzenini temsil eder. |
| [setSortAsNumber(boolean value)](#setSortAsNumber-boolean-) | Bir sayıya benzeyen şeylerin sıralanıp sıralanmayacağını gösterir. |
| [setSortLeftToRight(boolean value)](#setSortLeftToRight-boolean-) | Doğru, sıralama yönünün soldan sağa olduğunu gösterir. |
| [sort()](#sort--) | Aralıktaki verileri sırala. |
| [sort(Cells cells, CellArea area)](#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-) | Alan verilerini sırala. |
| [sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)](#sort-com.aspose.cells.Cells-int-int-int-int-) | Alan verilerini sıralar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addColorKey(int key, int type, int order, Color color) {#addColorKey-int-int-int-com.aspose.cells.Color-}
```
public void addColorKey(int key, int type, int order, Color color)
```


Renk sıralama anahtarını ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | int | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Sıralanmış renk değer tipi. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sıralama düzeni. |
| color | [Color](../../com.aspose.cells/color) | Özel sıralama rengi. |

### addKey(int key, int order) {#addKey-int-int-}
```
public void addKey(int key, int order)
```


Sıralanmış sütun indeksini ve sıralama düzenini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | int | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sıralama düzeni |

### addKey(int key, int type, int order, Object customList) {#addKey-int-int-int-java.lang.Object-}
```
public void addKey(int key, int type, int order, Object customList)
```


Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler.

**Remarks**

Tip SortOnType.CellColor veya SortOnType.FontColor ise, customList Color'dir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | int | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| type | int | [SortOnType](../../com.aspose.cells/sortontype). Sıralanmış değer tipi. |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sıralama düzeni. |
| customList | java.lang.Object | Özel sıralama listesi. |

### addKey(int key, int order, String customList) {#addKey-int-int-java.lang.String-}
```
public void addKey(int key, int order, String customList)
```


Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | int | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sıralama düzeni. |
| customList | java.lang.String | Özel sıralama listesi. |

### addKey(int key, int order, String[] customList) {#addKey-int-int-java.lang.String---}
```
public void addKey(int key, int order, String[] customList)
```


Özel sıralama listesiyle sıralanmış sütun indeksini ve sıralama düzenini ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| anahtar | int | Sıralanmış sütun indeksi (mutlak konum, A sütunu 0, B 1, ...) |
| order | int | [SortOrder](../../com.aspose.cells/sortorder). Sıralama düzeni. |
| customList | java.lang.String[] | Özel sıralama listesi. |

### clear() {#clear--}
```
public void clear()
```


Tüm ayarları temizle.

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
### getCaseSensitive() {#getCaseSensitive--}
```
public boolean getCaseSensitive()
```


Dize karşılaştırılırken büyük/küçük harfe duyarlı olup olmadığını alır.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getKey1() {#getKey1--}
```
public int getKey1()
```


İlk sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

**Returns:**
int
### getKey2() {#getKey2--}
```
public int getKey2()
```


İkinci sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

**Returns:**
int
### getKey3() {#getKey3--}
```
public int getKey3()
```


Üçüncü sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

**Returns:**
int
### getKeys() {#getKeys--}
```
public DataSorterKeyCollection getKeys()
```


Veri sıralayıcının anahtar listesini alır.

**Returns:**
[DataSorterKeyCollection](../../com.aspose.cells/datasorterkeycollection)
### getOrder1() {#getOrder1--}
```
public int getOrder1()
```


İlk anahtarın sıralama düzenini temsil eder.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Returns:**
int
### getOrder2() {#getOrder2--}
```
public int getOrder2()
```


İkinci anahtarın sıralama düzenini temsil eder.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Returns:**
int
### getOrder3() {#getOrder3--}
```
public int getOrder3()
```


Üçüncü anahtarın sıralama düzenini temsil eder.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Returns:**
int
### getSortAsNumber() {#getSortAsNumber--}
```
public boolean getSortAsNumber()
```


Bir sayıya benzeyen şeylerin sıralanıp sıralanmayacağını gösterir.

**Returns:**
boolean
### getSortLeftToRight() {#getSortLeftToRight--}
```
public boolean getSortLeftToRight()
```


True, sıralama yönünün soldan sağa olduğunu ifade eder. False, sıralama yönünün üstten alta olduğunu ifade eder. Varsayılan değer false'tur.

**Returns:**
boolean
### hasHeaders() {#hasHeaders--}
```
public boolean hasHeaders()
```


Aralığın başlık içerip içermediğini temsil eder.

**Returns:**
boolean
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




### setCaseSensitive(boolean value) {#setCaseSensitive-boolean-}
```
public void setCaseSensitive(boolean value)
```


Dize karşılaştırılırken büyük/küçük harfe duyarlı olup olmadığını ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setHasHeaders(boolean value) {#setHasHeaders-boolean-}
```
public void setHasHeaders(boolean value)
```


Aralığın başlık içerip içermediğini temsil eder.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setKey1(int value) {#setKey1-int-}
```
public void setKey1(int value)
```


İlk sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setKey2(int value) {#setKey2-int-}
```
public void setKey2(int value)
```


İkinci sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setKey3(int value) {#setKey3-int-}
```
public void setKey3(int value)
```


Üçüncü sıralanmış sütun indeksini temsil eder (mutlak konum, A sütunu 0, B 1, ...).

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOrder1(int value) {#setOrder1-int-}
```
public void setOrder1(int value)
```


İlk anahtarın sıralama düzenini temsil eder.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOrder2(int value) {#setOrder2-int-}
```
public void setOrder2(int value)
```


İkinci anahtarın sıralama düzenini temsil eder.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setOrder3(int value) {#setOrder3-int-}
```
public void setOrder3(int value)
```


Üçüncü anahtarın sıralama düzenini temsil eder.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setSortAsNumber(boolean value) {#setSortAsNumber-boolean-}
```
public void setSortAsNumber(boolean value)
```


Bir sayıya benzeyen şeylerin sıralanıp sıralanmayacağını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setSortLeftToRight(boolean value) {#setSortLeftToRight-boolean-}
```
public void setSortLeftToRight(boolean value)
```


True, sıralama yönünün soldan sağa olduğunu ifade eder. False, sıralama yönünün üstten alta olduğunu ifade eder. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### sort() {#sort--}
```
public int[] sort()
```


Aralıktaki verileri sırala.

**Returns:**
int[] - sıralanmış satırların/sütunların orijinal indeksleri (mutlak konum, örneğin A sütunu 0, B 1, ...) . Eğer bu sıralama işlemiyle taşınacak satır/sütun yoksa, null döndürülür.
### sort(Cells cells, CellArea area) {#sort-com.aspose.cells.Cells-com.aspose.cells.CellArea-}
```
public int[] sort(Cells cells, CellArea area)
```


Alan verilerini sırala.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Hücreler veri alanını içerir. |
| area | [CellArea](../../com.aspose.cells/cellarea) | Sıralanması gereken alan |

**Returns:**
int[] - sıralanmış satırların/sütunların orijinal indeksleri (mutlak konum, örneğin A sütunu 0, B 1, ...) . Eğer bu sıralama işlemiyle taşınacak satır/sütun yoksa, null döndürülür.
### sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn) {#sort-com.aspose.cells.Cells-int-int-int-int-}
```
public int[] sort(Cells cells, int startRow, int startColumn, int endRow, int endColumn)
```


Alan verilerini sıralar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cells | [Cells](../../com.aspose.cells/cells) | Hücreler veri alanını içerir. |
| startRow | int | Alan başlangıç satırı. |
| startColumn | int | Alan başlangıç sütunu. |
| endRow | int | Alan bitiş satırı. |
| endColumn | int | Alan bitiş sütunu. |

**Returns:**
int[] - sıralanmış satırların/sütunların orijinal indeksleri (mutlak konum, örneğin A sütunu 0, B 1, ...) . Eğer bu sıralama işlemiyle taşınacak satır/sütun yoksa, null döndürülür.
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

