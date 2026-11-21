---
title: "DataSorterKey"
second_title: "Aspose.Cells for Java API Referansı"
description: "Veri sıralayıcının anahtarını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/datasorterkey/
---

**Inheritance:**
java.lang.Object
```
public class DataSorterKey
```

Veri sıralayıcının anahtarını temsil eder.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | Sıralanmış rengi alır. |
| [getIconId()](#getIconId--) | Simge seti türünün kimliğini temsil eder. |
| [getIconSetType()](#getIconSetType--) | Simge seti türünü temsil eder. |
| [getIndex()](#getIndex--) | Sıralanmış sütun dizinini alır (mutlak konum, sütun A 0, B 1, ...). |
| [getOrder()](#getOrder--) | Sıralama düzenini gösterir. |
| [getType()](#getType--) | Sıralama tipini temsil eder. |
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
### getColor() {#getColor--}
```
public Color getColor()
```


Sıralanmış rengi alır.

**Remarks**

Yalnızca [getType()](../../com.aspose.cells/datasorterkey\#getType--) [SortOnType.CELL\_COLOR](../../com.aspose.cells/sortontype\#CELL-COLOR) veya [SortOnType.FONT\_COLOR](../../com.aspose.cells/sortontype\#FONT-COLOR) olduğunda etkili olur.

**Returns:**
[Color](../../com.aspose.cells/color)
### getIconId() {#getIconId--}
```
public int getIconId()
```


Simge seti türünün kimliğini temsil eder.

**Remarks**

Yalnızca [getType()](../../com.aspose.cells/datasorterkey\#getType--) [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON) olduğunda etkili olur.

**Returns:**
int
### getIconSetType() {#getIconSetType--}
```
public int getIconSetType()
```


Simge seti türünü temsil eder.

Bakınız [IconSetType](../../com.aspose.cells/iconsettype).

**Remarks**

Yalnızca [getType()](../../com.aspose.cells/datasorterkey\#getType--) [SortOnType.ICON](../../com.aspose.cells/sortontype\#ICON) olduğunda etkili olur.

**Returns:**
int
### getIndex() {#getIndex--}
```
public int getIndex()
```


Sıralanmış sütun dizinini alır (mutlak konum, sütun A 0, B 1, ...).

**Returns:**
int
### getOrder() {#getOrder--}
```
public int getOrder()
```


Sıralama düzenini gösterir.

[SortOrder](../../com.aspose.cells/sortorder) öğesine bakın.

**Returns:**
int
### getType() {#getType--}
```
public int getType()
```


Sıralama tipini temsil eder.

Bakınız [SortOnType](../../com.aspose.cells/sortontype).

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

