---
title: "FormatConditionCollection"
second_title: "Aspose.Cells for Java API Referansı"
description: "Koşullu biçimlendirmeyi temsil eder."
type: docs
url: /tr/java/com.aspose.cells/formatconditioncollection/
---

**Inheritance:**
java.lang.Object
```
public class FormatConditionCollection
```

Koşullu biçimlendirmeyi temsil eder. FormatConditions üç koşullu biçime kadar içerebilir.

**Example**

```
         //Create a new Workbook.
         Workbook workbook = new Workbook();
 
         //Get the first worksheet.
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
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
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
         //Adds condition.
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
| [add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)](#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-) | Bir biçimlendirme koşulu ve etkilenen hücre aralığını FormatConditions'a ekler. FormatConditions üç koşullu biçime kadar içerebilir. |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Koşullu biçimlendirilmiş bir hücre aralığı ekler. |
| [addCondition(int type)](#addCondition-int-) | Bir biçim koşulu ekle. |
| [addCondition(int type, int operatorType, String formula1, String formula2)](#addCondition-int-int-java.lang.String-java.lang.String-) | Bir biçimlendirme koşulu ekler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Biçimlendirme koşulunu indeksle alır. |
| [getCellArea(int index)](#getCellArea-int-) | Koşullu biçimlendirilmiş hücre aralığını indeksle alır. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Koşulların sayısını alır. |
| [getRangeCount()](#getRangeCount--) | Koşullu biçimlendirilmiş aralıkların sayısını alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeArea(int index)](#removeArea-int-) | Koşullu biçimlendirilmiş hücre aralığını indeksle kaldırır. |
| [removeArea(int startRow, int startColumn, int totalRows, int totalColumns)](#removeArea-int-int-int-int-) | Aralıktaki koşullu biçimlendirmeyi kaldır. |
| [removeCondition(int index)](#removeCondition-int-) | Biçimlendirme koşulunu indeksle kaldırır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add(CellArea cellArea, int type, int operatorType, String formula1, String formula2) {#add-com.aspose.cells.CellArea-int-int-java.lang.String-java.lang.String-}
```
public int[] add(CellArea cellArea, int type, int operatorType, String formula1, String formula2)
```


Bir biçimlendirme koşulu ve etkilenen hücre aralığını FormatConditions'a ekler. FormatConditions en fazla üç koşullu biçim içerebilir. Koşullu biçimlendirme formüllerinde diğer sayfalara referans verilmesine izin verilmez.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Koşullu biçimlendirilmiş hücre aralığı. |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Koşullu biçimlendirme türü. FormatConditionType üyesi olabilir. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Karşılaştırma operatörü. OperatorType üyesi olabilir. |
| formula1 | java.lang.String | Koşullu biçimlendirme ile ilişkili değer veya ifade. |
| formula2 | java.lang.String | Koşullu biçimlendirme ile ilişkili değer veya ifade |

**Returns:**
int[] - [0]:Biçimlendirme koşulu nesne indeksi;[1] Etkilenen hücre aralığı indeksi.
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public int addArea(CellArea cellArea)
```


Koşullu biçimlendirilmiş bir hücre aralığı ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | Koşullu biçimlendirilmiş hücre aralığı. |

**Returns:**
int - Koşullu biçimlendirilmiş hücre aralığı indeksi.
### addCondition(int type) {#addCondition-int-}
```
public int addCondition(int type)
```


Bir biçim koşulu ekle.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Biçim koşulu türü. |

**Returns:**
int - Biçimlendirme koşulu nesne indeksi;
### addCondition(int type, int operatorType, String formula1, String formula2) {#addCondition-int-int-java.lang.String-java.lang.String-}
```
public int addCondition(int type, int operatorType, String formula1, String formula2)
```


Bir biçimlendirme koşulu ekler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| type | int | [FormatConditionType](../../com.aspose.cells/formatconditiontype). Biçim koşulunun türü. |
| operatorType | int | [OperatorType](../../com.aspose.cells/operatortype). Operatör türü |
| formula1 | java.lang.String | Koşullu biçimlendirme ile ilişkili değer veya ifade. Giriş değeri '=' ile başlıyorsa, formül olarak kabul edilir. Aksi takdirde düz değer (metin, sayı, bool) olarak kabul edilir. '=' ile başlayan metin değeri, kullanıcı tarafından \"=\\\\\"=...\\\\\"\" biçiminde formül olarak girilebilir. |
| formula2 | java.lang.String | Koşullu biçimlendirme ile ilişkili değer veya ifade. Girdi biçimi formula1 ile aynı. |

**Returns:**
int - Biçimlendirme koşulu nesne indeksi;
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
public FormatCondition get(int index)
```


Biçimlendirme koşulunu indeksle alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | döndürülecek biçimlendirme koşulunun dizini. |

**Returns:**
[FormatCondition](../../com.aspose.cells/formatcondition) - the formatting condition
### getCellArea(int index) {#getCellArea-int-}
```
public CellArea getCellArea(int index)
```


Koşullu biçimlendirilmiş hücre aralığını indeksle alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | koşullu biçimlendirilmiş hücre aralığının dizini. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the conditional formatted cell range
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


Koşulların sayısını alır.

**Returns:**
int
### getRangeCount() {#getRangeCount--}
```
public int getRangeCount()
```


Koşullu biçimlendirilmiş aralıkların sayısını alır.

**Returns:**
int
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




### removeArea(int index) {#removeArea-int-}
```
public void removeArea(int index)
```


Koşullu biçimlendirilmiş hücre aralığını indeksle kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak koşullu biçimlendirilmiş hücre aralığının dizini. |

### removeArea(int startRow, int startColumn, int totalRows, int totalColumns) {#removeArea-int-int-int-int-}
```
public boolean removeArea(int startRow, int startColumn, int totalRows, int totalColumns)
```


Aralıktaki koşullu biçimlendirmeyi kaldır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Aralığın başlangıç satırı. |
| startColumn | int | Aralığın başlangıç sütunu. |
| totalRows | int | Aralıktaki satır sayısı. |
| totalColumns | int | Aralıktaki sütun sayısı. |

**Returns:**
boolean - TRUE döndürür, bu FormatCondtionCollection kaldırılmalıdır.
### removeCondition(int index) {#removeCondition-int-}
```
public void removeCondition(int index)
```


Biçimlendirme koşulunu indeksle kaldırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Kaldırılacak biçimlendirme koşulunun dizini. |

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

