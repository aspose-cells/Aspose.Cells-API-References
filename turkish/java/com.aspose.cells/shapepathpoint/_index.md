---
title: "ShapePathPoint"
second_title: "Aspose.Cells for Java API Referansı"
description: "konum koordinatlarını veya açı işaretçilerini belirtin."
type: docs
url: /tr/java/com.aspose.cells/shapepathpoint/
---

**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```

Pozisyon koordinatlarını veya açı işaretçilerini belirtin. Pozisyon koordinatları, bir koordinat uzayındaki yolun koordinatlarını temsil eder (ör. X/Y). Açı işaretçileri, bir yoldaki açısal değişimleri gösterir (ör. bir yayının başlangıç ve salınım açıları).
## Yöntemler

| Yöntem | Açıklama |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Geçerli nesnenin değer türünü belirtir. |
| [getX()](#getX--) | Bu pozisyon koordinatı için x koordinatını alır. |
| [getXAngle()](#getXAngle--) | Nesne bir açı işaretçisi olduğunda, derece cinsinden ilk açıyı al veya ayarla. |
| [getXPixel()](#getXPixel--) | Nesne bir pozisyon koordinatı olduğunda, piksel cinsinden x koordinatını al veya ayarla. |
| [getY()](#getY--) | Bu pozisyon koordinatı için y koordinatını alır. |
| [getYAngle()](#getYAngle--) | Nesne bir açı işaretçisi olduğunda, derece cinsinden ikinci açıyı al veya ayarla. |
| [getYPixel()](#getYPixel--) | Nesne bir pozisyon koordinatı olduğunda, piksel cinsinden y koordinatını al veya ayarla. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | Bu pozisyon koordinatı için x koordinatını ayarlar. |
| [setXAngle(int value)](#setXAngle-int-) | Nesne bir açı işaretçisi olduğunda, derece cinsinden ilk açıyı al veya ayarla. |
| [setXPixel(int value)](#setXPixel-int-) | Nesne bir pozisyon koordinatı olduğunda, piksel cinsinden x koordinatını al veya ayarla. |
| [setY(int value)](#setY-int-) | Bu pozisyon koordinatı için y koordinatını alır. |
| [setYAngle(int value)](#setYAngle-int-) | Nesne bir açı işaretçisi olduğunda, derece cinsinden ikinci açıyı al veya ayarla. |
| [setYPixel(int value)](#setYPixel-int-) | Nesne bir pozisyon koordinatı olduğunda, piksel cinsinden y koordinatını al veya ayarla. |
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
### getType() {#getType--}
```
public int getType()
```


Geçerli nesnenin değer türünü belirtir.

Bak [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype).

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


Bu pozisyon koordinatı için x koordinatını alır. Birim EMU.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ShapePathPoint.XPixel ve ShapePathPoint.XAngle özelliklerini kullanın. Bu özellik, Ağustos 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```


Nesne bir açı işaretçisi olduğunda, derece cinsinden ilk açıyı al veya ayarla.

**Remarks**

Bu açı bir yay başlangıç açısıysa. Bu açı, varsayılan daire yolunda yay çizimi için başlangıç konumu olarak kullanılacak açıyı belirler. Bu başlangıç açısı, şekil yolundaki son bilinen kalem konumuna kilitlenir. Böylece kesintisiz bir şekil yolu garantilenir.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


Nesne bir pozisyon koordinatı olduğunda, piksel cinsinden x koordinatını al veya ayarla.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


Bu konum koordinatı için y koordinatını alır. Birim EMU.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ShapePathPoint.YPixel ve ShapePathPoint.YAngle özelliklerini kullanın. Bu özellik, Ağustos 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```


Nesne bir açı işaretçisi olduğunda, derece cinsinden ikinci açıyı al veya ayarla.

**Remarks**

Bu açı bir yay salınım açısıysa. Bu açı, varsayılan daire yolunda yay ne kadar açıyla uzatılacağını belirler. Başlangıç açısından yapılan uzatma her zaman varsayılan daire etrafında saat yönünde olacaktır.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


Nesne bir pozisyon koordinatı olduğunda, piksel cinsinden y koordinatını al veya ayarla.

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




### setX(int value) {#setX-int-}
```
public void setX(int value)
```


Bu konum koordinatı için x koordinatını ayarlar. Birim EMU.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ShapePathPoint.XPixel ve ShapePathPoint.XAngle özelliklerini kullanın. Bu özellik, Ağustos 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```


Nesne bir açı işaretçisi olduğunda, derece cinsinden ilk açıyı al veya ayarla.

**Remarks**

Bu açı bir yay başlangıç açısıysa. Bu açı, varsayılan daire yolunda yay çizimi için başlangıç konumu olarak kullanılacak açıyı belirler. Bu başlangıç açısı, şekil yolundaki son bilinen kalem konumuna kilitlenir. Böylece kesintisiz bir şekil yolu garantilenir.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


Nesne bir pozisyon koordinatı olduğunda, piksel cinsinden x koordinatını al veya ayarla.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


Bu konum koordinatı için y koordinatını alır. Birim EMU.

**Remarks**

NOT: Bu üye artık kullanımdan kaldırıldı. Bunun yerine lütfen ShapePathPoint.YPixel ve ShapePathPoint.YAngle özelliklerini kullanın. Bu özellik, Ağustos 2025'ten itibaren 12 ay sonra kaldırılacak. Aspose, yaşadığınız herhangi bir rahatsızlıktan dolayı özür diler.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```


Nesne bir açı işaretçisi olduğunda, derece cinsinden ikinci açıyı al veya ayarla.

**Remarks**

Bu açı bir yay salınım açısıysa. Bu açı, varsayılan daire yolunda yay ne kadar açıyla uzatılacağını belirler. Başlangıç açısından yapılan uzatma her zaman varsayılan daire etrafında saat yönünde olacaktır.

**Parameters:**
| Parametre | Tür | Açıklama |
| --- | --- | --- |
| değer | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


Nesne bir pozisyon koordinatı olduğunda, piksel cinsinden y koordinatını al veya ayarla.

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

