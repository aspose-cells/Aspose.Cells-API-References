---
title: "ConditionalFormattingCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Nesnelerin bir koleksiyonunu kapsar."
type: docs
url: /tr/java/com.aspose.cells/conditionalformattingcollection/
---

**Inheritance:**
java.lang.Object, [com.aspose.cells.CollectionBase](../../com.aspose.cells/collectionbase)
```
public class ConditionalFormattingCollection extends CollectionBase
```

Bir [FormatCondition](../../com.aspose.cells/formatcondition) nesnelerinin koleksiyonunu kapsüller.

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
 
         //Add condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
         //Add condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         //Saving the Excel file
         workbook.save("output.xls");
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [add()](#add--) | Koleksiyona bir FormatConditions ekler. |
| [add(Object o)](#add-java.lang.Object-) | CollectionBase örneğine bir öğe ekler. |
| [clear()](#clear--) | CollectionBase örneğinden tüm nesneleri kaldırır. |
| [contains(Object o)](#contains-java.lang.Object-) | Örneğin bu nesneyi içerip içermediğini döndürür |
| [copy(ConditionalFormattingCollection cfs)](#copy-com.aspose.cells.ConditionalFormattingCollection-) | Koşullu biçimlendirmeyi kopyalar. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Belirtilen dizindeki FormatConditions öğesini alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | CollectionBase örneğinde bulunan eleman sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [indexOf(Object o)](#indexOf-java.lang.Object-) | CollectionBase örneğindeki belirli bir öğenin dizinini belirler. |
| [iterator()](#iterator--) | CollectionBase örneği üzerinde yineleme yapan bir enumerator döndürür. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Aralıktaki tüm koşullu biçimlendirmeyi kaldır. |
| [removeAt(int index)](#removeAt-int-) | Belirtilen dizindeki öğeyi kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public int add()
```


Koleksiyona bir FormatConditions ekler.

**Returns:**
int - FormatConditions nesne indeksi.
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
### copy(ConditionalFormattingCollection cfs) {#copy-com.aspose.cells.ConditionalFormattingCollection-}
```
public void copy(ConditionalFormattingCollection cfs)
```


Koşullu biçimlendirmeyi kopyalar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cfs | [ConditionalFormattingCollection](../../com.aspose.cells/conditionalformattingcollection) | Koşullu biçimlendirme |

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
public FormatConditionCollection get(int index)
```


Belirtilen dizindeki FormatConditions öğesini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Öğenin sıfır tabanlı indeksi. |

**Returns:**
[FormatConditionCollection](../../com.aspose.cells/formatconditioncollection)
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




### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public void removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


Aralıktaki tüm koşullu biçimlendirmeyi kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Aralığın başlangıç satırı. |
| startColumn | int | Aralığın başlangıç sütunu. |
| totalRows | int | Aralıktaki satır sayısı. |
| totalColumns | int | Aralıktaki sütun sayısı. |

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

