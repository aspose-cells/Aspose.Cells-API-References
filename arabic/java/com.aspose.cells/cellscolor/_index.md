---
title: "CellsColor"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل جميع أنواع الألوان."
type: docs
url: /ar/java/com.aspose.cells/cellscolor/
---

**Inheritance:**
java.lang.Object
```
public class CellsColor
```

يمثل جميع أنواع الألوان.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getArgb()](#getArgb--) | يحصل على اللون من قيمة ARGB 32‑بت. |
| [getClass()](#getClass--) |  |
| [getColor()](#getColor--) | يحصل على اللون RGB. |
| [getColorIndex()](#getColorIndex--) | يحصل على فهرس اللون في لوحة الألوان. |
| [getThemeColor()](#getThemeColor--) | يحصل على لون السمة. |
| [getTransparency()](#getTransparency--) | يحصل على الشفافية كقيمة تتراوح بين 0.0 (معتم) إلى 1.0 (شفاف). |
| [getType()](#getType--) | نوع اللون. |
| [hashCode()](#hashCode--) |  |
| [isShapeColor()](#isShapeColor--) | يحصل على اللون الذي يجب تطبيقه على الخلية أو الشكل. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setArgb(int value)](#setArgb-int-) | يضبط اللون من قيمة ARGB 32‑بت. |
| [setColor(Color value)](#setColor-com.aspose.cells.Color-) | يضبط لون RGB. |
| [setColorIndex(int value)](#setColorIndex-int-) | يضبط فهرس اللون في لوحة الألوان. |
| [setShapeColor(boolean value)](#setShapeColor-boolean-) | يضبط اللون الذي يجب تطبيقه على الخلية أو الشكل. |
| [setThemeColor(ThemeColor value)](#setThemeColor-com.aspose.cells.ThemeColor-) | يحصل على لون السمة. |
| [setTintOfShapeColor(double tint)](#setTintOfShapeColor-double-) | ضبط درجة لون الشكل |
| [setTransparency(double value)](#setTransparency-double-) | يضبط الشفافية كقيمة تتراوح بين 0.0 (معتم) إلى 1.0 (شفاف). |
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
### getArgb() {#getArgb--}
```
public int getArgb()
```


يحصل على اللون من قيمة ARGB 32‑بت.

**Returns:**
int
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


يحصل على اللون RGB.

**Returns:**
[Color](../../com.aspose.cells/color)
### getColorIndex() {#getColorIndex--}
```
public int getColorIndex()
```


يحصل على فهرس اللون في لوحة الألوان. ينطبق فقط على اللون المفهرس.

**Returns:**
int
### getThemeColor() {#getThemeColor--}
```
public ThemeColor getThemeColor()
```


يحصل على لون السمة. ينطبق فقط على نوع لون السمة.

**Returns:**
[ThemeColor](../../com.aspose.cells/themecolor)
### getTransparency() {#getTransparency--}
```
public double getTransparency()
```


يحصل على الشفافية كقيمة تتراوح بين 0.0 (معتم) إلى 1.0 (شفاف).

**Returns:**
double
### getType() {#getType--}
```
public int getType()
```


نوع اللون.

انظر [ColorType](../../com.aspose.cells/colortype).

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isShapeColor() {#isShapeColor--}
```
public boolean isShapeColor()
```


يحصل على اللون الذي يجب تطبيقه على الخلية أو الشكل.

**Remarks**

تعبير لون الخلية والشكل مختلف. على سبيل المثال: لون السمة مع نفس قيمة الدرجة لن يكون هو نفسه في الخلية والشكل.

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




### setArgb(int value) {#setArgb-int-}
```
public void setArgb(int value)
```


يضبط اللون من قيمة ARGB 32‑بت.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setColor(Color value) {#setColor-com.aspose.cells.Color-}
```
public void setColor(Color value)
```


يضبط لون RGB.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.cells/color) |  |

### setColorIndex(int value) {#setColorIndex-int-}
```
public void setColorIndex(int value)
```


يضبط فهرس اللون في لوحة الألوان. ينطبق فقط على اللون المفهرس.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShapeColor(boolean value) {#setShapeColor-boolean-}
```
public void setShapeColor(boolean value)
```


يضبط اللون الذي يجب تطبيقه على الخلية أو الشكل.

**Remarks**

تعبير لون الخلية والشكل مختلف. على سبيل المثال: لون السمة مع نفس قيمة الدرجة لن يكون هو نفسه في الخلية والشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setThemeColor(ThemeColor value) {#setThemeColor-com.aspose.cells.ThemeColor-}
```
public void setThemeColor(ThemeColor value)
```


يحصل على لون السمة. ينطبق فقط على نوع لون السمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [ThemeColor](../../com.aspose.cells/themecolor) |  |

### setTintOfShapeColor(double tint) {#setTintOfShapeColor-double-}
```
public void setTintOfShapeColor(double tint)
```


ضبط درجة لون الشكل

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| tint | double |  |

### setTransparency(double value) {#setTransparency-double-}
```
public void setTransparency(double value)
```


يضبط الشفافية كقيمة تتراوح بين 0.0 (معتم) إلى 1.0 (شفاف).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

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

