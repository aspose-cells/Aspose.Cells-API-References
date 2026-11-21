---
title: "CalculationCell"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hesaplanan bir hücreyle ilgili hesaplama verilerini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/calculationcell/
---

**Inheritance:**
java.lang.Object
```
public class CalculationCell
```

Hesaplanan bir hücreyle ilgili hesaplama verilerini temsil eder.

**Remarks**

Kullanıcı, formül hesaplama süreci sırasında Çalışma Kitabı'ndaki herhangi bir veriyi değiştirmemelidir, aksi takdirde beklenmeyen sonuçlar veya İstisna oluşabilir. Bu nedenle, bu sınıf tarafından sağlanan tüm nesneler (örneğin [getCell()](../../com.aspose.cells/calculationcell\\#getCell--) metodunun Cell nesnesi gibi) yalnızca \"read\" amaçlıdır.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCell()](#getCell--) | Hesaplanan Cell nesnesini alır. |
| [getCellColumn()](#getCellColumn--) | Hücrenin sütun indeksini alır. |
| [getCellRow()](#getCellRow--) | Hücrenin satır indeksini alır. |
| [getClass()](#getClass--) |  |
| [getWorkbook()](#getWorkbook--) | Workbook nesnesini alır. |
| [getWorksheet()](#getWorksheet--) | Hücrenin bulunduğu Worksheet nesnesini alır. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object v)](#setCalculatedValue-java.lang.Object-) | Hücre için hesaplanan değeri ayarlar. |
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
### getCell() {#getCell--}
```
public Cell getCell()
```


Hesaplanan Cell nesnesini alır.

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


Hücrenin sütun indeksini alır.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


Hücrenin satır indeksini alır.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


Workbook nesnesini alır.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


Hücrenin bulunduğu Worksheet nesnesini alır.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object v) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object v)
```


Hücre için hesaplanan değeri ayarlar.

**Remarks**

Kullanıcı, hücre için otomatik hesaplamayı yok saymak amacıyla bu yöntemle hesaplanmış sonucu ayarlayabilir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| v | java.lang.Object |  |

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

