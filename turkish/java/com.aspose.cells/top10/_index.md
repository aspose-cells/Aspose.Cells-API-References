---
title: "Top10"
second_title: "Aspose.Cells for Java API Referansı"
description: "Top10 koşullu biçimlendirme kuralını açıklar."
type: docs
url: /tr/java/com.aspose.cells/top10/
---

**Inheritance:**
java.lang.Object
```
public class Top10
```

Top10 koşullu biçimlendirme kuralını açıklayın. Bu koşullu biçimlendirme kuralı, değerleri belirtilen üst N veya alt N aralığına düşen hücreleri vurgular.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = CellArea.createCellArea(0, 0, 10, 10);
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.TOP_10, OperatorType.NONE, null, null);   
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
         Top10 top10 = fc.getTop10();
         //Set the Top N 
         top10.setRank(5);  
         //Saving the Excel file
         workbook.save("output.xls");
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [Top10()](#Top10--) |  |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getRank()](#getRank--) | Bir "üst/alt n" koşullu biçimlendirme kuralında "n" değerini alır. |
| [hashCode()](#hashCode--) |  |
| [isBottom()](#isBottom--) | Bir "top/bottom n" kuralının "bottom n" kuralı olup olmadığını alır. |
| [isPercent()](#isPercent--) | Bir "top/bottom n" kuralının "top/bottom n percent" kuralı olup olmadığını alır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBottom(boolean value)](#setBottom-boolean-) | Bir "top/bottom n" kuralının "bottom n" kuralı olup olmadığını ayarlar. |
| [setPercent(boolean value)](#setPercent-boolean-) | Bir "top/bottom n" kuralının "top/bottom n percent" kuralı olup olmadığını ayarlar. |
| [setRank(int value)](#setRank-int-) | "top/bottom n" koşullu biçimlendirme kuralındaki "n" değerini ayarlar. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### Top10() {#Top10--}
```
public Top10()
```


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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getRank() {#getRank--}
```
public int getRank()
```


"top/bottom n" koşullu biçimlendirme kuralındaki "n" değerini alır. IsPercent doğru ise, değer 0 ile 100 arasında olmalıdır. Aksi takdirde 0 ile 1000 arasında olmalıdır. Varsayılan değer 10'dur.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBottom() {#isBottom--}
```
public boolean isBottom()
```


Bir "top/bottom n" kuralının "bottom n" kuralı olup olmadığını alır. Varsayılan değer false'tur.

**Returns:**
boolean
### isPercent() {#isPercent--}
```
public boolean isPercent()
```


Bir "top/bottom n" kuralının "top/bottom n percent" kuralı olup olmadığını alır. Varsayılan değer false'tur.

**Returns:**
boolean
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setBottom(boolean value) {#setBottom-boolean-}
```
public void setBottom(boolean value)
```


Bir "top/bottom n" kuralının "bottom n" kuralı olup olmadığını ayarlar. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setPercent(boolean value) {#setPercent-boolean-}
```
public void setPercent(boolean value)
```


Bir "top/bottom n" kuralının "top/bottom n percent" kuralı olup olmadığını ayarlar. Varsayılan değer false'tur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setRank(int value) {#setRank-int-}
```
public void setRank(int value)
```


"top/bottom n" koşullu biçimlendirme kuralındaki "n" değerini ayarlar. IsPercent doğru ise, değer 0 ile 100 arasında olmalıdır. Aksi takdirde 0 ile 1000 arasında olmalıdır. Varsayılan değer 10'dur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

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

