---
title: "RenderingWatermark"
second_title: "Aspose.Cells for Java API Reference"
description: "علامة مائية للعرض."
type: docs
url: /ar/java/com.aspose.cells/renderingwatermark/
---

**Inheritance:**
java.lang.Object
```
public class RenderingWatermark
```

علامة مائية للعرض.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [RenderingWatermark(String text, RenderingFont renderingFont)](#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-) | إنشاء مثيل للعلامة المائية النصية. |
| [RenderingWatermark(byte[] imageData)](#RenderingWatermark-byte---) | إنشاء مثيل للعلامة المائية الصورة. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getFont()](#getFont--) | يحصل على خط العلامة المائية. |
| [getHAlignment()](#getHAlignment--) | يحصل على المحاذاة الأفقية للعلامة المائية بالنسبة للصفحة. |
| [getImage()](#getImage--) | يحصل على صورة العلامة المائية. |
| [getOffsetX()](#getOffsetX--) | يحصل على قيمة الإزاحة إلى [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [getOffsetY()](#getOffsetY--) | يحصل على قيمة الإزاحة إلى [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [getOpacity()](#getOpacity--) | يحصل على شفافية العلامة المائية في النطاق [0, 1]. |
| [getRotation()](#getRotation--) | يحصل على دوران العلامة المائية بالدرجات. |
| [getScaleToPagePercent()](#getScaleToPagePercent--) | يحصل على مقياس العلامة المائية نسبةً إلى الصفحة المستهدفة بالنسبة المئوية. |
| [getText()](#getText--) | يحصل على نص العلامة المائية. |
| [getVAlignment()](#getVAlignment--) | يحصل على المحاذاة العمودية للعلامة المائية بالنسبة للصفحة. |
| [hashCode()](#hashCode--) |  |
| [isBackground()](#isBackground--) | يشير إلى ما إذا كانت العلامة المائية موضوعة خلف محتويات الصفحة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBackground(boolean value)](#setBackground-boolean-) | يشير إلى ما إذا كانت العلامة المائية موضوعة خلف محتويات الصفحة. |
| [setHAlignment(int value)](#setHAlignment-int-) | يضبط المحاذاة الأفقية للعلامة المائية بالنسبة للصفحة. |
| [setOffsetX(float value)](#setOffsetX-float-) | يضبط قيمة الإزاحة إلى [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--) |
| [setOffsetY(float value)](#setOffsetY-float-) | يضبط قيمة الإزاحة إلى [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--) |
| [setOpacity(float value)](#setOpacity-float-) | يضبط شفافية العلامة المائية في النطاق [0, 1]. |
| [setRotation(float value)](#setRotation-float-) | يضبط دوران العلامة المائية بالدرجات. |
| [setScaleToPagePercent(int value)](#setScaleToPagePercent-int-) | يضبط مقياس العلامة المائية نسبةً إلى الصفحة المستهدفة بالنسبة المئوية. |
| [setVAlignment(int value)](#setVAlignment-int-) | يضبط المحاذاة العمودية للعلامة المائية بالنسبة للصفحة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### RenderingWatermark(String text, RenderingFont renderingFont) {#RenderingWatermark-java.lang.String-com.aspose.cells.RenderingFont-}
```
public RenderingWatermark(String text, RenderingFont renderingFont)
```


إنشاء مثيل للعلامة المائية النصية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| نص | java.lang.String | نص العلامة المائية |
| renderingFont | [RenderingFont](../../com.aspose.cells/renderingfont) | خط العلامة المائية |

### RenderingWatermark(byte[] imageData) {#RenderingWatermark-byte---}
```
public RenderingWatermark(byte[] imageData)
```


إنشاء مثيل للعلامة المائية الصورة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| imageData | byte[] |  |

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
### getFont() {#getFont--}
```
public RenderingFont getFont()
```


يحصل على خط العلامة المائية.

**Returns:**
[RenderingFont](../../com.aspose.cells/renderingfont)
### getHAlignment() {#getHAlignment--}
```
public int getHAlignment()
```


يحصل على المحاذاة الأفقية للعلامة المائية بالنسبة للصفحة.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

فقط Left, Center, Right صالحة. الافتراضي هو Left.

**Returns:**
int
### getImage() {#getImage--}
```
public byte[] getImage()
```


يحصل على صورة العلامة المائية.

**Returns:**
byte[]
### getOffsetX() {#getOffsetX--}
```
public float getOffsetX()
```


يحصل على قيمة الإزاحة إلى [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Returns:**
float
### getOffsetY() {#getOffsetY--}
```
public float getOffsetY()
```


يحصل على قيمة الإزاحة إلى [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Returns:**
float
### getOpacity() {#getOpacity--}
```
public float getOpacity()
```


يحصل على شفافية العلامة المائية في النطاق [0, 1].

**Returns:**
float
### getRotation() {#getRotation--}
```
public float getRotation()
```


يحصل على دوران العلامة المائية بالدرجات.

**Returns:**
float
### getScaleToPagePercent() {#getScaleToPagePercent--}
```
public int getScaleToPagePercent()
```


يحصل على مقياس العلامة المائية نسبةً إلى الصفحة المستهدفة بالنسبة المئوية.

**Returns:**
int
### getText() {#getText--}
```
public String getText()
```


يحصل على نص العلامة المائية.

**Returns:**
java.lang.String
### getVAlignment() {#getVAlignment--}
```
public int getVAlignment()
```


يحصل على المحاذاة العمودية للعلامة المائية بالنسبة للصفحة.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

فقط Top, Center, Bottom صالحة. الافتراضي هو Top.

**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isBackground() {#isBackground--}
```
public boolean isBackground()
```


يشير إلى ما إذا كانت العلامة المائية موضوعة خلف محتويات الصفحة.

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




### setBackground(boolean value) {#setBackground-boolean-}
```
public void setBackground(boolean value)
```


يشير إلى ما إذا كانت العلامة المائية موضوعة خلف محتويات الصفحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setHAlignment(int value) {#setHAlignment-int-}
```
public void setHAlignment(int value)
```


يضبط المحاذاة الأفقية للعلامة المائية بالنسبة للصفحة.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

فقط Left, Center, Right صالحة. الافتراضي هو Left.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setOffsetX(float value) {#setOffsetX-float-}
```
public void setOffsetX(float value)
```


يضبط قيمة الإزاحة إلى [getHAlignment()](../../com.aspose.cells/renderingwatermark\#getHAlignment--)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setOffsetY(float value) {#setOffsetY-float-}
```
public void setOffsetY(float value)
```


يضبط قيمة الإزاحة إلى [getVAlignment()](../../com.aspose.cells/renderingwatermark\#getVAlignment--)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setOpacity(float value) {#setOpacity-float-}
```
public void setOpacity(float value)
```


يضبط شفافية العلامة المائية في النطاق [0, 1].

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setRotation(float value) {#setRotation-float-}
```
public void setRotation(float value)
```


يضبط دوران العلامة المائية بالدرجات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | float |  |

### setScaleToPagePercent(int value) {#setScaleToPagePercent-int-}
```
public void setScaleToPagePercent(int value)
```


يضبط مقياس العلامة المائية نسبةً إلى الصفحة المستهدفة بالنسبة المئوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setVAlignment(int value) {#setVAlignment-int-}
```
public void setVAlignment(int value)
```


يضبط المحاذاة العمودية للعلامة المائية بالنسبة للصفحة.

انظر [TextAlignmentType](../../com.aspose.cells/textalignmenttype).

**Remarks**

فقط Top, Center, Bottom صالحة. الافتراضي هو Top.

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

