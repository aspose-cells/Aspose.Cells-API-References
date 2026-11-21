---
title: "HorizontalPageBreak"
second_title: "Aspose.Cells for Java API Referansı"
description: "Yatay sayfa sonunu temsil eden nesneyi kapsüller."
type: docs
url: /tr/java/com.aspose.cells/horizontalpagebreak/
---

**Inheritance:**
java.lang.Object
```
public class HorizontalPageBreak
```

Yatay sayfa sonunu temsil eden nesneyi kapsüller.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         //Obtaining the reference of the newly added worksheet by passing its sheet index
         Worksheet worksheet = workbook.getWorksheets().get(0);
 
         //Add a page break at cell Y30
         int Index = worksheet.getHorizontalPageBreaks().add("Y30");
 
         //get the newly added horizontal page break
         HorizontalPageBreak hPageBreak = worksheet.getHorizontalPageBreaks().get(Index);
```
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Bu yatay sayfa sonlandırıcısının son sütun dizinini alır. |
| [getRow()](#getRow--) | Sıfır tabanlı satır dizinini alır. |
| [getStartColumn()](#getStartColumn--) | Bu yatay sayfa sonlandırıcısının başlangıç sütun dizinini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


Bu yatay sayfa sonlandırıcısının son sütun dizinini alır.

**Returns:**
int
### getRow() {#getRow--}
```
public int getRow()
```


Sıfır tabanlı satır dizinini alır.

**Returns:**
int
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Bu yatay sayfa sonlandırıcısının başlangıç sütun dizinini alır.

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

