---
title: "ShapePath"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل مسار إنشاء يتكون من سلسلة من خطوط الحركة والمنحنيات التي عند دمجها ستشكل شكلًا هندسيًا."
type: docs
url: /ar/java/com.aspose.cells/shapepath/
---

**Inheritance:**
java.lang.Object
```
public class ShapePath
```

يمثل مسار إنشاء يتكون من سلسلة من الحركات والخطوط والمنحنيات التي عند دمجها ستشكل شكلاً هندسياً.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [ShapePath()](#ShapePath--) | يُهيئ نسخة جديدة من الفئة [ShapePath](../../com.aspose.cells/shapepath). |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [arcTo(float wR, float hR, float stAng, float swAng)](#arcTo-float-float-float-float-) | يضيف قوسًا بيضاويًا إلى الشكل الحالي. |
| [close()](#close--) | يغلق الشكل الحالي ويبدأ شكلًا جديدًا. |
| [cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)](#cubicBezierTo-float-float-float-float-float-float-) | يضيف منحنى B\u8305zier مكعب إلى الشكل الحالي. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getHeightPixel()](#getHeightPixel--) | يحصل على ارتفاع هذا المسار بوحدة البكسل. |
| [getPathSegementList()](#getPathSegementList--) | يحصل على قائمة [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getPathSegments()](#getPathSegments--) | يحصل على قائمة [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection). |
| [getWidthPixel()](#getWidthPixel--) | يحصل على عرض هذا المسار بوحدة البكسل. |
| [hashCode()](#hashCode--) |  |
| [lineTo(float x, float y)](#lineTo-float-float-) | يضيف قطعة خط إلى الشكل الحالي. |
| [moveTo(float x, float y)](#moveTo-float-float-) | يبدأ شكلًا جديدًا من النقطة المحددة دون إغلاق الشكل الحالي. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setHeightPixel(int value)](#setHeightPixel-int-) | يحصل على ارتفاع هذا المسار بوحدة البكسل. |
| [setWidthPixel(int value)](#setWidthPixel-int-) | يحصل على عرض هذا المسار بوحدة البكسل. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ShapePath() {#ShapePath--}
```
public ShapePath()
```


يُهيئ نسخة جديدة من الفئة [ShapePath](../../com.aspose.cells/shapepath).

### arcTo(float wR, float hR, float stAng, float swAng) {#arcTo-float-float-float-float-}
```
public void arcTo(float wR, float hR, float stAng, float swAng)
```


يضيف قوسًا بيضاويًا إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| wR | float | نصف عرض المنطقة المستطيلة للبيضاوي \\u9225\\u5b27\\u20ac\\u5aa1 الذي يرسم القوس (الوحدة: بكسل). |
| hR | float | نصف ارتفاع المنطقة المستطيلة للبيضاوي \\u9225\\u5b27\\u20ac\\u5aa1 الذي يرسم القوس (الوحدة: بكسل). |
| stAng | float | زاوية البداية للقوس، تُقاس بالدرجات في اتجاه عقارب الساعة من محور x (الوحدة: درجة). ستحدد هذه الزاوية أي زاوية على مسار الدائرة المفترض سيتم استخدامها كنقطة بدء لرسم القوس. سيتم قفل زاوية البداية هذه إلى آخر موضع قلم معروف في مسار الشكل، مما يضمن مسار شكل مستمر. |
| swAng | float | زاوية التأرجح للقوس. ستحدد هذه الزاوية مدى الامتداد الزاوي على مسار الدائرة المفترض. الامتداد من زاوية البداية سيكون دائمًا في اتجاه عقارب الساعة حول الدائرة المفترض (الوحدة: درجة). |

### close() {#close--}
```
public void close()
```


يغلق الشكل الحالي ويبدأ شكلًا جديدًا. إذا كان الشكل الحالي يحتوي على سلسلة من الخطوط والمنحنيات المتصلة، فإن الطريقة تغلق الحلقة بربط خط من نقطة النهاية إلى نقطة البداية.

### cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY) {#cubicBezierTo-float-float-float-float-float-float-}
```
public void cubicBezierTo(float ctrX1, float ctrY1, float ctrX2, float ctrY2, float endX, float endY)
```


يضيف منحنى بيزيه مكعب B\\u8305 إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. الوحدة: بكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ctrX1 | float | الإحداثي السيني للنقطة التحكمية الأولى للمنحنى (الوحدة: بكسل). |
| ctrY1 | float | الإحداثي الصادي للنقطة التحكمية الأولى للمنحنى (الوحدة: بكسل). |
| ctrX2 | float | الإحداثي السيني للنقطة التحكمية الثانية للمنحنى (الوحدة: بكسل). |
| ctrY2 | float | الإحداثي الصادي للنقطة التحكمية الثانية للمنحنى (الوحدة: بكسل). |
| endX | float | الإحداثي السيني لنقطة النهاية للمنحنى (الوحدة: بكسل). |
| endY | float | الإحداثي الصادي لنقطة النهاية للمنحنى (الوحدة: بكسل). |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| معامل | نوع | الوصف |
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


يحصل على ارتفاع هذا المسار بوحدة البكسل.

**Returns:**
int
### getPathSegementList() {#getPathSegementList--}
```
public ShapeSegmentPathCollection getPathSegementList()
```


يحصل على قائمة [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية ShapePath.PathSegments. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يوليو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getPathSegments() {#getPathSegments--}
```
public ShapeSegmentPathCollection getPathSegments()
```


يحصل على قائمة [ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection).

**Returns:**
[ShapeSegmentPathCollection](../../com.aspose.cells/shapesegmentpathcollection)
### getWidthPixel() {#getWidthPixel--}
```
public int getWidthPixel()
```


يحصل على عرض هذا المسار بوحدة البكسل.

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


يضيف مقطع خط إلى الشكل الحالي. نقطة البداية هي نقطة النهاية للشكل الحالي. الوحدة: بكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| x | float | الإحداثي السيني لنقطة النهاية لمقطع الخط (الوحدة: بكسل). |
| y | float | الإحداثي الصادي لنقطة النهاية لمقطع الخط (الوحدة: بكسل). |

### moveTo(float x, float y) {#moveTo-float-float-}
```
public void moveTo(float x, float y)
```


يبدأ شكلاً جديدًا من النقطة المحددة دون إغلاق الشكل الحالي. جميع النقاط اللاحقة التي تُضاف إلى المسار تُضاف إلى هذا الشكل الجديد. الوحدة: بكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| x | float | الإحداثي السيني لنقطة بدء الشكل (الوحدة: بكسل). |
| y | float | الإحداثي الصادي لنقطة بدء الشكل (الوحدة: بكسل). |

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


يحصل على ارتفاع هذا المسار بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setWidthPixel(int value) {#setWidthPixel-int-}
```
public void setWidthPixel(int value)
```


يحصل على عرض هذا المسار بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

