---
title: "TextBoxOptions"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل خيارات النص للشكل"
type: docs
url: /ar/java/com.aspose.cells/textboxoptions/
---

**Inheritance:**
java.lang.Object
```
public class TextBoxOptions
```

يمثل خيارات النص للشكل

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         int index = workbook.getWorksheets().get(0).getTextBoxes().add(0, 0, 350, 350);
         Shape shape = workbook.getWorksheets().get(0).getTextBoxes().get(index);
         shape.setText("This is test.");
 
         //do your business
 
         //Save the excel file.
         workbook.save("exmaple.xlsx");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowTextToOverflow()](#getAllowTextToOverflow--) | ما إذا كان يسمح للنص بتجاوز الشكل. |
| [getBottomMarginPt()](#getBottomMarginPt--) | يعيد الهامش السفلي بوحدة النقاط |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | يحصل على الهامش الأيسر بوحدة النقاط. |
| [getResizeToFitText()](#getResizeToFitText--) | يشير إلى ما إذا كان يجب تغيير حجم الشكل ليتناسب مع النص |
| [getRightMarginPt()](#getRightMarginPt--) | يحصل على الهامش الأيمن بوحدة النقاط. |
| [getShapeTextDirection()](#getShapeTextDirection--) | يحصل على اتجاه عرض النص داخل جسم نص معين. |
| [getShapeTextVerticalAlignment()](#getShapeTextVerticalAlignment--) | يتوافق مع "تنسيق الشكل - خيارات النص - مربع النص - المحاذاة العمودية" في Excel. |
| [getTopMarginPt()](#getTopMarginPt--) | يحصل على الهامش العلوي بوحدة النقاط. |
| [getWrapTextInShape()](#getWrapTextInShape--) | يحدد لف النص داخل الشكل. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowTextToOverflow(boolean value)](#setAllowTextToOverflow-boolean-) | ما إذا كان يسمح للنص بتجاوز الشكل. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | يعيد الهامش السفلي بوحدة النقاط |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | يضبط الهامش الأيسر بوحدة النقاط. |
| [setResizeToFitText(boolean value)](#setResizeToFitText-boolean-) | يشير إلى ما إذا كان يجب تغيير حجم الشكل ليتناسب مع النص |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | يضبط الهامش الأيمن بوحدة النقاط. |
| [setShapeTextDirection(int value)](#setShapeTextDirection-int-) | يضبط اتجاه عرض النص داخل جسم نص معين. |
| [setShapeTextVerticalAlignment(int value)](#setShapeTextVerticalAlignment-int-) | يتوافق مع "تنسيق الشكل - خيارات النص - مربع النص - المحاذاة العمودية" في Excel. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | يضبط الهامش العلوي بوحدة النقاط. |
| [setWrapTextInShape(boolean value)](#setWrapTextInShape-boolean-) | يحدد لف النص داخل الشكل. |
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
### getAllowTextToOverflow() {#getAllowTextToOverflow--}
```
public boolean getAllowTextToOverflow()
```


ما إذا كان يسمح للنص بتجاوز الشكل.

**Example**

```
         shape.getTextBoxOptions().setAllowTextToOverflow(true);
```

**Returns:**
boolean
### getBottomMarginPt() {#getBottomMarginPt--}
```
public double getBottomMarginPt()
```


يعيد الهامش السفلي بوحدة النقاط

**Example**

```
         shape.getTextBoxOptions().setBottomMarginPt(0.2d);
```

**Returns:**
double
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getLeftMarginPt() {#getLeftMarginPt--}
```
public double getLeftMarginPt()
```


يحصل على الهامش الأيسر بوحدة النقاط.

**Example**

```
         shape.getTextBoxOptions().setLeftMarginPt(0.2d);
```

**Returns:**
double
### getResizeToFitText() {#getResizeToFitText--}
```
public boolean getResizeToFitText()
```


يشير إلى ما إذا كان يجب تغيير حجم الشكل ليتناسب مع النص

**Example**

```
         shape.getTextBoxOptions().setResizeToFitText(true);
```

**Returns:**
boolean
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


يحصل على الهامش الأيمن بوحدة النقاط.

**Example**

```
         shape.getTextBoxOptions().setRightMarginPt(0.2d);
```

**Returns:**
double
### getShapeTextDirection() {#getShapeTextDirection--}
```
public int getShapeTextDirection()
```


يحصل على اتجاه عرض النص داخل جسم نص معين. يتطابق مع "Format Shape - Text Options - Text Box - Text direction" في Excel

انظر [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Example**

```
         shape.getTextBoxOptions().setShapeTextDirection(TextVerticalType.VERTICAL);
```

**Returns:**
int
### getShapeTextVerticalAlignment() {#getShapeTextVerticalAlignment--}
```
public int getShapeTextVerticalAlignment()
```


يتوافق مع "تنسيق الشكل - خيارات النص - مربع النص - المحاذاة العمودية" في Excel.

انظر [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Example**

```
         shape.getTextBoxOptions().setShapeTextVerticalAlignment(ShapeTextVerticalAlignmentType.LEFT);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


يحصل على الهامش العلوي بوحدة النقاط.

**Example**

```
         shape.getTextBoxOptions().setTopMarginPt(0.2d);
```

**Returns:**
double
### getWrapTextInShape() {#getWrapTextInShape--}
```
public boolean getWrapTextInShape()
```


يحدد لف النص داخل الشكل. False - لا يحدث لف في جسم النص. True - يحدث لف في جسم النص.

**Example**

```
         shape.getTextBoxOptions().setWrapTextInShape(true);
```

**Returns:**
boolean
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




### setAllowTextToOverflow(boolean value) {#setAllowTextToOverflow-boolean-}
```
public void setAllowTextToOverflow(boolean value)
```


ما إذا كان يسمح للنص بتجاوز الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setBottomMarginPt(double value) {#setBottomMarginPt-double-}
```
public void setBottomMarginPt(double value)
```


يعيد الهامش السفلي بوحدة النقاط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLeftMarginPt(double value) {#setLeftMarginPt-double-}
```
public void setLeftMarginPt(double value)
```


يضبط الهامش الأيسر بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setResizeToFitText(boolean value) {#setResizeToFitText-boolean-}
```
public void setResizeToFitText(boolean value)
```


يشير إلى ما إذا كان يجب تغيير حجم الشكل ليتناسب مع النص

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


يضبط الهامش الأيمن بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setShapeTextDirection(int value) {#setShapeTextDirection-int-}
```
public void setShapeTextDirection(int value)
```


يضبط اتجاه عرض النص داخل جسم نص معين. يتطابق مع "Format Shape - Text Options - Text Box - Text direction" في Excel

انظر [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setShapeTextVerticalAlignment(int value) {#setShapeTextVerticalAlignment-int-}
```
public void setShapeTextVerticalAlignment(int value)
```


يتوافق مع "تنسيق الشكل - خيارات النص - مربع النص - المحاذاة العمودية" في Excel.

انظر [ShapeTextVerticalAlignmentType](../../com.aspose.cells/shapetextverticalalignmenttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


يضبط الهامش العلوي بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setWrapTextInShape(boolean value) {#setWrapTextInShape-boolean-}
```
public void setWrapTextInShape(boolean value)
```


يحدد لف النص داخل الشكل. False - لا يحدث لف في جسم النص. True - يحدث لف في جسم النص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

