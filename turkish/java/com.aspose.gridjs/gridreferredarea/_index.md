---
title: "GridReferredArea"
second_title: "Aspose.Cells for Java API Referansı"
description: "Formül tarafından başvurulan bir alanı temsil eder."
type: docs
url: /tr/java/com.aspose.gridjs/gridreferredarea/
---

**Inheritance:**
java.lang.Object
```
public class GridReferredArea
```

Formül tarafından başvurulan bir alanı temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | Alan bitiş sütunu. |
| [getEndRow()](#getEndRow--) | Alan bitiş satırı. |
| [getExternalFileName()](#getExternalFileName--) | Bu bir dış referans ise dış dosya adını al. |
| [getSheetName()](#getSheetName--) | Bu sayfanın hangi sayfada olduğunu gösterir |
| [getStartColumn()](#getStartColumn--) | Alan başlangıç sütunu. |
| [getStartRow()](#getStartRow--) | Alan başlangıç satırı. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | Bu alanın sol üst köşesinden verilen offset ile hücre değerini alır. |
| [getValues()](#getValues--) | Bu alandaki hücre değerlerini alır. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | Bunun bir alan olup olmadığını gösterir. |
| [isExternalLink()](#isExternalLink--) | Bunun harici bir bağlantı olup olmadığını gösterir. |
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


Alan bitiş sütunu.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


Alan bitiş satırı.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


Bu bir dış referans ise dış dosya adını al.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Bu sayfanın hangi sayfada olduğunu gösterir

**Returns:**
java.lang.String
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


Alan başlangıç sütunu.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


Alan başlangıç satırı.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


Bu alanın sol üst köşesinden verilen offset ile hücre değerini alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| rowOffset | int | Bu alanın başlangıç satırından satır offset'i. |
| colOffset | int | Bu alanın başlangıç satırından sütun offset'i. |

**Returns:**
java.lang.Object - Alan geçersizse "\#REF!"; verilen offset bu alanın dışındaysa "\#N/A"; Aksi takdirde verilen konumdaki hücre değerini döndürür.
### getValues() {#getValues--}
```
public Object getValues()
```


Bu alandaki hücre değerlerini alır.

**Returns:**
java.lang.Object - Bu alan geçersizse, "\#REF!" döndürülür; Bu alan tek bir hücre ise, hücre değer nesnesi döndürülür; Aksi takdirde bu alandaki tüm değerler için bir dizi döndürülür.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


Bunun bir alan olup olmadığını gösterir.

**Remarks**

Bu bir alan değilse, yalnızca StartRow ve StartColumn etkili olur.

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


Bunun harici bir bağlantı olup olmadığını gösterir.

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

