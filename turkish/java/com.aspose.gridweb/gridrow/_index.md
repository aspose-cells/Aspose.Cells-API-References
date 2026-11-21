---
title: "GridRow"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir elektronik tabloda tek bir resmi temsil eden nesneyi kapsar."
type: docs
url: /tr/java/com.aspose.gridweb/gridrow/
---

**Inheritance:**
java.lang.Object
```
public class GridRow
```

Bir elektronik tabloda tek bir resmi temsil eden nesneyi kapsar.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int column)](#get-int-) | Hücreyi alır. |
| [getCellByIndex(int index)](#getCellByIndex-int-) | Listedeki belirli indeks ile hücreyi al. |
| [getClass()](#getClass--) |  |
| [getFirstCell()](#getFirstCell--) | Satırdaki ilk hücreyi alır. |
| [getHeight()](#getHeight--) | Satır yüksekliğini Point biriminde alır. |
| [getHidden()](#getHidden--) | Satırın gizli olup olmadığını gösterir. |
| [getIndex()](#getIndex--) | Bu satırın indeksini alır. |
| [getLastCell()](#getLastCell--) | Satırdaki son hücreyi alır. |
| [getLastDataCell()](#getLastDataCell--) | Satırdaki son hücreyi alır. |
| [getOutlineLevel()](#getOutlineLevel--) | Anahat seviyesini alır. |
| [hashCode()](#hashCode--) |  |
| [isBlank()](#isBlank--) | Satırın herhangi bir veri içerip içermediğini gösterir |
| [iterator()](#iterator--) | Hücre enumerator'ünü alır |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeight(double value)](#setHeight-double-) | Satır yüksekliğini Nokta biriminde ayarlar. |
| [setHidden(boolean value)](#setHidden-boolean-) | Satırın gizli olup olmadığını gösterir. |
| [setOutlineLevel(byte value)](#setOutlineLevel-byte-) | Anahat seviyesini ayarlar. |
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
### get(int column) {#get-int-}
```
public GridCell get(int column)
```


Hücreyi alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| sütun | int | Sütun indeksi |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - 
### getCellByIndex(int index) {#getCellByIndex-int-}
```
public GridCell getCellByIndex(int index)
```


Listedeki belirli indeks ile hücreyi al.

**Remarks**

NOT: Bu üye artık kullanılmıyor. Bunun yerine, bu satırdaki tüm hücreleri yinelemek için Row.GetEnumerator() metodunu kullanın. Bu özellik Şubat 2015'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| dizin | int | Pozisyon. |

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell) - The Cell object.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFirstCell() {#getFirstCell--}
```
public GridCell getFirstCell()
```


Satırdaki ilk hücreyi alır.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHeight() {#getHeight--}
```
public double getHeight()
```


Satır yüksekliğini Point biriminde alır.

**Returns:**
double
### getHidden() {#getHidden--}
```
public boolean getHidden()
```


Satırın gizli olup olmadığını gösterir.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


Bu satırın indeksini alır.

**Returns:**
int
### getLastCell() {#getLastCell--}
```
public GridCell getLastCell()
```


Satırdaki son hücreyi alır.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getLastDataCell() {#getLastDataCell--}
```
public GridCell getLastDataCell()
```


Satırdaki son hücreyi alır.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getOutlineLevel() {#getOutlineLevel--}
```
public byte getOutlineLevel()
```


Anahat seviyesini alır.

**Returns:**
byte
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBlank() {#isBlank--}
```
public boolean isBlank()
```


Satırın herhangi bir veri içerip içermediğini gösterir

**Returns:**
boolean
### iterator() {#iterator--}
```
public Iterator iterator()
```


Hücre enumerator'ünü alır

**Returns:**
java.util.Iterator - Hücre enumeratörü
### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeight(double value) {#setHeight-double-}
```
public void setHeight(double value)
```


Satır yüksekliğini Nokta biriminde ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | double |  |

### setHidden(boolean value) {#setHidden-boolean-}
```
public void setHidden(boolean value)
```


Satırın gizli olup olmadığını gösterir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | boolean |  |

### setOutlineLevel(byte value) {#setOutlineLevel-byte-}
```
public void setOutlineLevel(byte value)
```


Anahat seviyesini ayarlar.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | byte |  |

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

