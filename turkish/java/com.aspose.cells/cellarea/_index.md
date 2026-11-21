---
title: "CellArea"
second_title: "Aspose.Cells for Java API Referansı"
description: "Hücrelerin bir alanını temsil eder."
type: docs
url: /tr/java/com.aspose.cells/cellarea/
---

**Inheritance:**
java.lang.Object

**All Implemented Interfaces:**
java.lang.Comparable
```
public final class CellArea implements Comparable
```

Hücrelerin bir alanını temsil eder.

**Example**

```
         //Create Cell Area
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
```
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [CellArea()](#CellArea--) |  |
## Alanlar

| Alan | Açıklama |
| --- | --- |
| [EndColumn](#EndColumn) | Bu alanın son sütununu alır veya ayarlar. |
| [EndRow](#EndRow) | Bu alanın son satırını alır veya ayarlar. |
| [StartColumn](#StartColumn) | Bu alanın başlangıç sütununu alır veya ayarlar. |
| [StartRow](#StartRow) | Bu alanın başlangıç satırını alır veya ayarlar. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [compareTo(Object obj)](#compareTo-java.lang.Object-) | İki CellArea nesnesini üst‑sol köşelerine göre karşılaştırır. |
| [createCellArea(int startRow, int startColumn, int endRow, int endColumn)](#createCellArea-int-int-int-int-) | Bir hücre alanı oluşturur. |
| [createCellArea(String startCellName, String endCellName)](#createCellArea-java.lang.String-java.lang.String-) | Bir hücre alanı oluşturur. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | Geçerli hücre alanı nesnesini temsil eden bir dize döndürür. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellArea() {#CellArea--}
```
public CellArea()
```


### EndColumn {#EndColumn}
```
public int EndColumn
```


Bu alanın son sütununu alır veya ayarlar.

### EndRow {#EndRow}
```
public int EndRow
```


Bu alanın son satırını alır veya ayarlar.

### StartColumn {#StartColumn}
```
public int StartColumn
```


Bu alanın başlangıç sütununu alır veya ayarlar.

### StartRow {#StartRow}
```
public int StartRow
```


Bu alanın başlangıç satırını alır veya ayarlar.

### compareTo(Object obj) {#compareTo-java.lang.Object-}
```
public int compareTo(Object obj)
```


İki CellArea nesnesini üst‑sol köşelerine göre karşılaştırır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| obj | java.lang.Object |  |

**Returns:**
int - İki köşe farklı satırlardaysa, satır indekslerini karşılaştır. Aksi takdirde sütun indekslerini karşılaştır. İki köşe aynıysa, 0 döndürülür.
### createCellArea(int startRow, int startColumn, int endRow, int endColumn) {#createCellArea-int-int-int-int-}
```
public static CellArea createCellArea(int startRow, int startColumn, int endRow, int endColumn)
```


Bir hücre alanı oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startRow | int | Başlangıç satırı. |
| startColumn | int | Başlangıç sütunu. |
| endRow | int | Bitiş satırı. |
| endColumn | int | Bitiş sütunu. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
### createCellArea(String startCellName, String endCellName) {#createCellArea-java.lang.String-java.lang.String-}
```
public static CellArea createCellArea(String startCellName, String endCellName)
```


Bir hücre alanı oluşturur.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| startCellName | java.lang.String | Aralığın sol üst hücresi. |
| endCellName | java.lang.String | Aralığın sağ alt hücresi. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - Return a [CellArea](../../com.aspose.cells/cellarea).
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


Geçerli hücre alanı nesnesini temsil eden bir dize döndürür.

**Returns:**
java.lang.String -
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

