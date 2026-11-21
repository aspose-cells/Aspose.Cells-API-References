---
title: "ConditionalFormattingIconCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir nesne koleksiyonunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/conditionalformattingiconcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ConditionalFormattingIconCollection extends CollectionBase
```

Bir [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) nesnesi koleksiyonunu temsil eder.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
         //Get Conditional Formatting
         ConditionalFormattingCollection cformattings = sheet.getConditionalFormattings();
         //Adds an empty conditional formatting
         int index = cformattings.add();
         //Get newly added Conditional formatting
         FormatConditionCollection fcs = cformattings.get(index);
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
         //Sets condition
         int idx = fcs.addCondition(FormatConditionType.ICON_SET);
         FormatCondition cond = fcs.get(idx);
         //Sets condition's type
         cond.getIconSet().setType(IconSetType.ARROWS_GRAY_3);
         //Add custom iconset condition.
         ConditionalFormattingIcon cfIcon = cond.getIconSet().getCfIcons().get(0);
         cfIcon.setType(IconSetType.ARROWS_3);
         cfIcon.setIndex(0);
         ConditionalFormattingIcon cfIcon1 = cond.getIconSet().getCfIcons().get(1);
         cfIcon1.setType(IconSetType.ARROWS_GRAY_3);
         cfIcon1.setIndex(1);
         ConditionalFormattingIcon cfIcon2 = cond.getIconSet().getCfIcons().get(2);
         cfIcon2.setType(IconSetType.BOXES_5);
         cfIcon2.setIndex(2);
         //Saving the Excel file
         workbook.save("output.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add(ConditionalFormattingIcon cficon)](#add-com.aspose.cells.ConditionalFormattingIcon-) | Bir [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) nesnesi ekler. |
| [add(int type, int index)](#add-int-int-) | Bir [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) nesnesi ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen indeksteki ConditionalFormattingIcon öğesini alır. |
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
### add(ConditionalFormattingIcon cficon) {#add-com.aspose.cells.ConditionalFormattingIcon-}
```
public int add(ConditionalFormattingIcon cficon)
```


Bir [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) nesnesi ekler.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine, lütfen Add(IconSetType, int) yöntemini kullanın. Bu yöntem, Aralık 2025'ten itibaren 6 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cficon | [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) | Listedeki yeni nesnenin dizinini döndürür. |

**Returns:**
int
### add(int type, int index) {#add-int-int-}
```
public int add(int type, int index)
```


Bir [ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) nesnesi ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [IconSetType](../../com.aspose.cells/iconsettype). Değer tipi. |
| dizin | int | İndeks. |

**Returns:**
int - Listedeki yeni nesnenin dizinini döndürür.
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
public ConditionalFormattingIcon get(int index)
```


Belirtilen indeksteki ConditionalFormattingIcon öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[ConditionalFormattingIcon](../../com.aspose.cells/conditionalformattingicon) - The element at the specified index.
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

