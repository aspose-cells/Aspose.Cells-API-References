---
title: "ShapePathPoint"
second_title: "Aspose.Cells for Java API Reference"
description: "حدد إحداثيات الموقع أو علامات الزاوية."
type: docs
url: /ar/java/com.aspose.cells/shapepathpoint/
---

**Inheritance:**
java.lang.Object
```
public class ShapePathPoint
```

حدد إحداثيات الموقع أو علامات الزاوية. تمثل إحداثيات الموقع إحداثيات مسار في مساحة إحداثية (مثال: X/Y). تشير علامات الزاوية إلى تغييرات زاوية في مسار (مثال: زاوية البداية وزاوية الانحراف لقوس).
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | يحدد نوع القيمة للكائن الحالي. |
| [getX()](#getX--) | يحصل على إحداثي x لهذا الإحداثي الموقع. |
| [getXAngle()](#getXAngle--) | عندما يكون الكائن علامة زاوية، احصل أو عيّن الزاوية الأولى بالدرجات. |
| [getXPixel()](#getXPixel--) | عندما يكون الكائن إحداثيًا موقعًا، احصل أو عيّن إحداثي x بالبكسل. |
| [getY()](#getY--) | يحصل على إحداثي y لهذا الإحداثي الموقع. |
| [getYAngle()](#getYAngle--) | عندما يكون الكائن علامة زاوية، احصل أو عيّن الزاوية الثانية بالدرجات. |
| [getYPixel()](#getYPixel--) | عندما يكون الكائن إحداثيًا موقعًا، احصل أو عيّن إحداثي y بالبكسل. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setX(int value)](#setX-int-) | يضبط إحداثي x لهذا الإحداثي الموقع. |
| [setXAngle(int value)](#setXAngle-int-) | عندما يكون الكائن علامة زاوية، احصل أو عيّن الزاوية الأولى بالدرجات. |
| [setXPixel(int value)](#setXPixel-int-) | عندما يكون الكائن إحداثيًا موقعًا، احصل أو عيّن إحداثي x بالبكسل. |
| [setY(int value)](#setY-int-) | يحصل على إحداثي y لهذا الإحداثي الموقع. |
| [setYAngle(int value)](#setYAngle-int-) | عندما يكون الكائن علامة زاوية، احصل أو عيّن الزاوية الثانية بالدرجات. |
| [setYPixel(int value)](#setYPixel-int-) | عندما يكون الكائن إحداثيًا موقعًا، احصل أو عيّن إحداثي y بالبكسل. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getType() {#getType--}
```
public int getType()
```


يحدد نوع القيمة للكائن الحالي.

انظر [ShapePathPointValueType](../../com.aspose.cells/shapepathpointvaluetype).

**Returns:**
int
### getX() {#getX--}
```
public int getX()
```


يحصل على إحداثي x لهذا الإحداثي الموقع. الوحدة EMUs.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خصائص ShapePathPoint.XPixel و ShapePathPoint.XAngle. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getXAngle() {#getXAngle--}
```
public int getXAngle()
```


عندما يكون الكائن علامة زاوية، احصل أو عيّن الزاوية الأولى بالدرجات.

**Remarks**

إذا كان هذا الزاوية هي زاوية البداية لقوس. ستحدد هذه الزاوية أي زاوية على طول مسار الدائرة المفترض سيتم استخدامها كنقطة البداية لرسم القوس. سيتم قفل زاوية البداية إلى آخر موضع قلم معروف في مسار الشكل. وبالتالي يضمن مسار شكل مستمر.

**Returns:**
int
### getXPixel() {#getXPixel--}
```
public int getXPixel()
```


عندما يكون الكائن إحداثيًا موقعًا، احصل أو عيّن إحداثي x بالبكسل.

**Returns:**
int
### getY() {#getY--}
```
public int getY()
```


يحصل على إحداثي y لهذا الإحداثي الموضع. الوحدة EMUs.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خصائص ShapePathPoint.YPixel و ShapePathPoint.YAngle. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
int
### getYAngle() {#getYAngle--}
```
public int getYAngle()
```


عندما يكون الكائن علامة زاوية، احصل أو عيّن الزاوية الثانية بالدرجات.

**Remarks**

إذا كان هذا الزاوية هي زاوية التأرجح لقوس. ستحدد هذه الزاوية إلى أي مدى على طول مسار الدائرة المفترض سيتم تمديد القوس. الامتداد من زاوية البداية سيكون دائمًا في الاتجاه مع عقارب الساعة حول الدائرة المفترض.

**Returns:**
int
### getYPixel() {#getYPixel--}
```
public int getYPixel()
```


عندما يكون الكائن إحداثيًا موقعًا، احصل أو عيّن إحداثي y بالبكسل.

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


يضبط إحداثي x لهذا الإحداثي الموضع. الوحدة EMUs.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خصائص ShapePathPoint.XPixel و ShapePathPoint.XAngle. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setXAngle(int value) {#setXAngle-int-}
```
public void setXAngle(int value)
```


عندما يكون الكائن علامة زاوية، احصل أو عيّن الزاوية الأولى بالدرجات.

**Remarks**

إذا كان هذا الزاوية هي زاوية البداية لقوس. ستحدد هذه الزاوية أي زاوية على طول مسار الدائرة المفترض سيتم استخدامها كنقطة البداية لرسم القوس. سيتم قفل زاوية البداية إلى آخر موضع قلم معروف في مسار الشكل. وبالتالي يضمن مسار شكل مستمر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setXPixel(int value) {#setXPixel-int-}
```
public void setXPixel(int value)
```


عندما يكون الكائن إحداثيًا موقعًا، احصل أو عيّن إحداثي x بالبكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setY(int value) {#setY-int-}
```
public void setY(int value)
```


يحصل على إحداثي y لهذا الإحداثي الموضع. الوحدة EMUs.

**Remarks**

ملاحظة: هذا العضو الآن مهمل. بدلاً من ذلك، يرجى استخدام خصائص ShapePathPoint.YPixel و ShapePathPoint.YAngle. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أغسطس 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setYAngle(int value) {#setYAngle-int-}
```
public void setYAngle(int value)
```


عندما يكون الكائن علامة زاوية، احصل أو عيّن الزاوية الثانية بالدرجات.

**Remarks**

إذا كان هذا الزاوية هي زاوية التأرجح لقوس. ستحدد هذه الزاوية إلى أي مدى على طول مسار الدائرة المفترض سيتم تمديد القوس. الامتداد من زاوية البداية سيكون دائمًا في الاتجاه مع عقارب الساعة حول الدائرة المفترض.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setYPixel(int value) {#setYPixel-int-}
```
public void setYPixel(int value)
```


عندما يكون الكائن إحداثيًا موقعًا، احصل أو عيّن إحداثي y بالبكسل.

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

