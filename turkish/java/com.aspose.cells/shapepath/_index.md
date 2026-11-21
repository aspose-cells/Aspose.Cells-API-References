---
title: "ShapePath"
second_title: "Aspose.Cells for Java API Referansı"
description: "Bir dizi hareket çizgisi ve eğriden oluşan ve birleştirildiğinde geometrik bir şekil oluşturan bir oluşturma yolunu temsil eder."
type: docs
url: /tr/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

Bir dizi hareket, çizgi ve eğriden oluşan ve birleştirildiğinde geometrik bir şekil oluşturacak bir oluşturma yolunu temsil eder.
## Yapıcılar

| Yapıcı | Açıklama |
| --- | --- |
| [ShapePath()](#ShapePath--) | [ShapePath](../../com.aspose.cells/shapepath) sınıfının yeni bir örneğini başlatır. |
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | Mevcut şekle eliptik bir yay ekler. |
| [close()](#close--) | Mevcut şekli kapatır ve yeni bir şekil başlatır. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | Mevcut şekle kübik B\u8305zier eğrisi ekler. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | Bu yolun yüksekliğini piksel biriminde alır. |
| [getPathSegementList()](#getPathSegementList--) | [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) listesini alır |
| [getPathSegments()](#getPathSegments--) | [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) listesini alır |
| [getWidthPixel()](#getWidthPixel--) | Bu yolun genişliğini piksel biriminde alır. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | Mevcut şekle bir çizgi segmenti ekler. |
| [moveTo(float x, float y)](#moveTo-float-float-) | Mevcut şekli kapatmadan belirtilen noktadan yeni bir şekil başlatır. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | Bu yolun yüksekliğini piksel biriminde alır. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | Bu yolun genişliğini piksel biriminde alır. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


[ShapePath](../../com.aspose.cells/shapepath) sınıfının yeni bir örneğini başlatır.

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


Mevcut şekle eliptik bir yay ekler. Başlangıç noktası, mevcut şeklin son noktasıdır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| wR | float | Yayı çizen \\u9225\\u5b27\\u20ac\\u5aa1he elipsin dikdörtgen alanının yarı genişliği (Birim: Piksel). |
| hR | float | Yayı çizen \\u9225\\u5b27\\u20ac\\u5aa1he elipsin dikdörtgen alanının yarı yüksekliği (Birim: Piksel). |
| stAng | float | Yayın başlangıç açısı, x ekseninden saat yönünde derece cinsinden ölçülür (Birim: Derece). Bu açı, yay çizilirken başlangıç konumu olarak kullanılacak dairesel yol üzerindeki açıyı belirler. Bu başlangıç açısı, şekil yolundaki son bilinen kalem konumuna kilitlenir. Böylece kesintisiz bir şekil yolu sağlanır. |
| swAng | float | Bir yay için salınım açısı. Bu açı, varsayılan daire yolunda yay ne kadar açıyla uzatılacağını belirler. Başlangıç açısından yapılan uzatma her zaman varsayılan daire etrafında saat yönünde olur. (Birim: Derece) |

### close() {#close--}
```
public void close()
```


Mevcut şekli kapatır ve yeni bir şekle başlar. Mevcut şekil bağlı çizgi ve eğrilerden oluşan bir dizi içeriyorsa, yöntem son noktayı başlangıç noktasına bir çizgiyle bağlayarak döngüyü kapatır.

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


Mevcut şekle kübik B\\u8305zier eğrisi ekler. Başlangıç noktası, mevcut şeklin son noktasıdır. Birim: Piksel.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| ctrX1 | float | Eğri için ilk kontrol noktasının x koordinatı (Birim: Piksel). |
| ctrY1 | float | Eğri için ilk kontrol noktasının y koordinatı (Birim: Piksel). |
| ctrX2 | float | Eğri için ikinci kontrol noktasının x koordinatı (Birim: Piksel). |
| ctrY2 | float | Eğri için ikinci kontrol noktasının y koordinatı (Birim: Piksel). |
| endX | float | Eğrinin son noktasının x koordinatı (Birim: Piksel). |
| endY | float | Eğrinin son noktasının y koordinatı (Birim: Piksel). |

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
### getHeightPixel() {#getHeightPixel--}
```
public int getHeightPixel()
```


Bu yolun yüksekliğini piksel biriminde alır.

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) listesini alır

**Remarks**

NOT: Bu üye artık kullanımdan kaldırılmıştır. Bunun yerine lütfen ShapePath.PathSegments özelliğini kullanın. Bu özellik Temmuz 2026'dan itibaren 12 ay sonra kaldırılacaktır. Aspose, yaşadığınız herhangi bir rahatsızlık için özür diler.

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection) listesini alır

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


Bu yolun genişliğini piksel biriminde alır.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### lineTo(float x, float y) {#lineTo-float-float-}
```
public void lineTo(float x, float y)
```


Mevcut şekle bir çizgi segmenti ekler. Başlangıç noktası, mevcut şeklin son noktasıdır. Birim: Piksel.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| x | float | Çizgi parçasının son noktasının x koordinatı (Birim: Piksel). |
| y | float | Çizgi parçasının son noktasının y koordinatı (Birim: Piksel). |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


Mevcut şekli kapatmadan belirtilen noktadan yeni bir şekil başlatır. Yola eklenen sonraki tüm noktalar bu yeni şekle eklenir. Birim: Piksel.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| x | float | Şeklin başlangıç noktasının x koordinatı (Birim: Piksel). |
| y | float | Şeklin başlangıç noktasının y koordinatı (Birim: Piksel). |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### setHeightPixel(int value) {#setHeightPixel-int-}
```
public void setHeightPixel(int value)
```


Bu yolun yüksekliğini piksel biriminde alır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


Bu yolun genişliğini piksel biriminde alır.

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

