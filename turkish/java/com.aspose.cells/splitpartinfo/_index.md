---
title: "SplitPartInfo"
second_title: "Aspose.Cells for Java API Referansı"
description: "Elektronik tabloyu görüntüye dönüştürürken işlenecek mevcut sayfa gibi birden çok giriş/çıkış için bir giriş/çıkış bilgisini temsil eder."
type: docs
url: /tr/java/com.aspose.cells/splitpartinfo/
---

**Inheritance:**
java.lang.Object
```
public class SplitPartInfo
```

Birden fazla giriş/çıkış için bir giriş/çıkış bilgisini temsil eder, örneğin elektronik tabloyu görüntüye dönüştürürken işlenecek mevcut sayfa.
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getPartIndex()](#getPartIndex--) | Sıradaki mevcut parçanın indeksi (0 tabanlı) |
| [getSheetIndex()](#getSheetIndex--) | Mevcut parçanın bulunduğu sayfanın indeksi. -1, yalnızca bir sayfa olduğunu gösterir. |
| [getSheetName()](#getSheetName--) | Mevcut parçanın bulunduğu sayfanın adı. |
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
### getPartIndex() {#getPartIndex--}
```
public int getPartIndex()
```


Sıradaki mevcut parçanın indeksi (0 tabanlı). -1, birden fazla parça olmadığını ve sonucun tek olduğunu gösterir.

**Remarks**

Birden fazla sayfa işlenmesi gerekiyorsa ve her sayfa ayrı ayrı (bölünerek) işleniyorsa, bölüm indeksi her sayfa için her zaman 0'dan başlar. Örneğin, çalışma kitabı görüntülere dönüştürülürken, şu anda işlenen sayfanın çıktı sayfa indeksini temsil eder. Ve -1, mevcut sayfa için yalnızca bir sayfa olduğunu gösterir.

**Returns:**
int
### getSheetIndex() {#getSheetIndex--}
```
public int getSheetIndex()
```


Mevcut parçanın bulunduğu sayfanın indeksi. -1, yalnızca bir sayfa olduğunu gösterir.

**Returns:**
int
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


Mevcut parçanın bulunduğu sayfanın adı.

**Remarks**

Bazı durumlarda, örneğin tüm çalışma kitabı tiff görüntüsü olarak render edildiğinde, null olabilir.

**Returns:**
java.lang.String
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

