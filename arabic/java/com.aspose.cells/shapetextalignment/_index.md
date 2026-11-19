---
title: "ShapeTextAlignment"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل إعداد محاذاة نص الأشكال"
type: docs
url: /ar/java/com.aspose.cells/shapetextalignment/
---

**Inheritance:**
java.lang.Object
```
public class ShapeTextAlignment
```

يمثل إعداد محاذاة نص الشكل؛

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Shape shape = workbook.getWorksheets().get(0).getShapes().addRectangle(1, 0, 1, 0, 50, 100);
         ShapeTextAlignment shapeTextAlignment = shape.getTextBody().getTextAlignment();
 
         //do your business
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object obj)](#equals-java.lang.Object-) | يحدد ما إذا كانت هذه الحالة لها نفس القيمة ككائن [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) المحدد الآخر. |
| [getAutoSize()](#getAutoSize--) | يشير إلى ما إذا كان حجم الشكل يتم ضبطه تلقائيًا وفقًا لمحتوياته. |
| [getBottomMarginPt()](#getBottomMarginPt--) | يعيد الهامش السفلي بوحدة النقاط |
| [getClass()](#getClass--) |  |
| [getLeftMarginPt()](#getLeftMarginPt--) | يعيد الهامش الأيسر بوحدة النقاط |
| [getNumberOfColumns()](#getNumberOfColumns--) | يحصل على عدد أعمدة النص في المستطيل المحيط. |
| [getRightMarginPt()](#getRightMarginPt--) | يعيد الهامش الأيمن بوحدة النقاط |
| [getRotateTextWithShape()](#getRotateTextWithShape--) | يشير إلى ما إذا كان النص يدور مع الشكل. |
| [getRotationAngle()](#getRotationAngle--) | يحصل على دوران الشكل. |
| [getTextHorizontalOverflow()](#getTextHorizontalOverflow--) | يحصل على نوع تجاوز النص الأفقي لصندوق النص. |
| [getTextShapeType()](#getTextShapeType--) | يحصل على نوع التحويل للنص. |
| [getTextVerticalOverflow()](#getTextVerticalOverflow--) | يحصل على نوع تجاوز النص العمودي لصندوق النص. |
| [getTextVerticalType()](#getTextVerticalType--) | يحصل على اتجاه النص. |
| [getTopMarginPt()](#getTopMarginPt--) | يعيد الهامش العلوي بوحدة النقاط |
| [hashCode()](#hashCode--) |  |
| [isAutoMargin()](#isAutoMargin--) | يشير إلى ما إذا كان هامش إطار النص تلقائيًا. |
| [isLockedText()](#isLockedText--) | يشير إلى ما إذا كان الشكل مقفلًا عندما تكون ورقة العمل محمية. |
| [isTextWrapped()](#isTextWrapped--) | يحصل على نوع التفاف النص للشكل الذي يحتوي على نص. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoMargin(boolean value)](#setAutoMargin-boolean-) | يشير إلى ما إذا كان هامش إطار النص تلقائيًا. |
| [setAutoSize(boolean value)](#setAutoSize-boolean-) | يشير إلى ما إذا كان حجم الشكل يتم ضبطه تلقائيًا وفقًا لمحتوياته. |
| [setBottomMarginPt(double value)](#setBottomMarginPt-double-) | يعيد الهامش السفلي بوحدة النقاط |
| [setLeftMarginPt(double value)](#setLeftMarginPt-double-) | يعيد الهامش الأيسر بوحدة النقاط |
| [setLockedText(boolean value)](#setLockedText-boolean-) | يشير إلى ما إذا كان الشكل مقفلًا عندما تكون ورقة العمل محمية. |
| [setNumberOfColumns(int value)](#setNumberOfColumns-int-) | يضبط عدد أعمدة النص في المستطيل المحيط. |
| [setRightMarginPt(double value)](#setRightMarginPt-double-) | يعيد الهامش الأيمن بوحدة النقاط |
| [setRotateTextWithShape(boolean value)](#setRotateTextWithShape-boolean-) | يشير إلى ما إذا كان النص يدور مع الشكل. |
| [setRotationAngle(double value)](#setRotationAngle-double-) | يضبط دوران الشكل. |
| [setTextHorizontalOverflow(int value)](#setTextHorizontalOverflow-int-) | يضبط نوع تجاوز النص الأفقي لصندوق النص. |
| [setTextShapeType(int value)](#setTextShapeType-int-) | يضبط نوع التحويل للنص. |
| [setTextVerticalOverflow(int value)](#setTextVerticalOverflow-int-) | يضبط نوع تجاوز النص العمودي لصندوق النص. |
| [setTextVerticalType(int value)](#setTextVerticalType-int-) | يضبط اتجاه النص. |
| [setTextWrapped(boolean value)](#setTextWrapped-boolean-) | يضبط نوع التفاف النص للشكل الذي يحتوي على نص. |
| [setTopMarginPt(double value)](#setTopMarginPt-double-) | يعيد الهامش العلوي بوحدة النقاط |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يحدد ما إذا كانت هذه الحالة لها نفس القيمة ككائن [ShapeTextAlignment](../../com.aspose.cells/shapetextalignment) المحدد الآخر.

**Example**

```
         //You have to make sure that the index value in this line of code exists
         ShapeTextAlignment obj = workbook.getWorksheets().get(0).getShapes().get(0).getTextBody().getTextAlignment();
         if (shapeTextAlignment.equals(obj))
         {
             //do what you want
         }
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | كائن [ShapeTextAlignment] للمقارنة مع هذه الحالة. |

**Returns:**
boolean - true إذا كانت قيمة المعامل obj هي نفسها قيمة هذا الكائن؛ وإلا false. إذا كان obj يساوي null، تُعيد هذه الطريقة false.
### getAutoSize() {#getAutoSize--}
```
public boolean getAutoSize()
```


يشير إلى ما إذا كان حجم الشكل يتم ضبطه تلقائيًا وفقًا لمحتوياته.

**Example**

```
         shapeTextAlignment.setAutoSize(false);
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
         shapeTextAlignment.setBottomMarginPt(2.0d);
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


يعيد الهامش الأيسر بوحدة النقاط

**Example**

```
         shapeTextAlignment.setLeftMarginPt(2.0d);
```

**Returns:**
double
### getNumberOfColumns() {#getNumberOfColumns--}
```
public int getNumberOfColumns()
```


يحصل على عدد أعمدة النص في المستطيل المحيط.

**Returns:**
int
### getRightMarginPt() {#getRightMarginPt--}
```
public double getRightMarginPt()
```


يعيد الهامش الأيمن بوحدة النقاط

**Example**

```
         shapeTextAlignment.setRightMarginPt(2.0d);
```

**Returns:**
double
### getRotateTextWithShape() {#getRotateTextWithShape--}
```
public boolean getRotateTextWithShape()
```


يشير إلى ما إذا كان النص يدور مع الشكل.

**Example**

```
         shapeTextAlignment.setRotateTextWithShape(true);
```

**Returns:**
boolean
### getRotationAngle() {#getRotationAngle--}
```
public double getRotationAngle()
```


يحصل على دوران الشكل.

**Example**

```
         shapeTextAlignment.setRotationAngle(90);
```

**Returns:**
double
### getTextHorizontalOverflow() {#getTextHorizontalOverflow--}
```
public int getTextHorizontalOverflow()
```


يحصل على نوع تجاوز النص الأفقي لصندوق النص.

انظر [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         shapeTextAlignment.setTextHorizontalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextShapeType() {#getTextShapeType--}
```
public int getTextShapeType()
```


يحصل على نوع التحويل للنص.

انظر [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Example**

```
         //Usually do not modify this value unless you know exactly what the modification will result in
         shapeTextAlignment.setTextShapeType(AutoShapeType.TEXT_BOX);
```

**Returns:**
int
### getTextVerticalOverflow() {#getTextVerticalOverflow--}
```
public int getTextVerticalOverflow()
```


يحصل على نوع تجاوز النص العمودي لصندوق النص.

انظر [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Example**

```
         shapeTextAlignment.setTextVerticalOverflow(TextOverflowType.CLIP);
```

**Returns:**
int
### getTextVerticalType() {#getTextVerticalType--}
```
public int getTextVerticalType()
```


يحصل على اتجاه النص.

انظر [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Example**

```
         shapeTextAlignment.setTextVerticalType(com.aspose.cells.TextVerticalType.HORIZONTAL);
```

**Returns:**
int
### getTopMarginPt() {#getTopMarginPt--}
```
public double getTopMarginPt()
```


يعيد الهامش العلوي بوحدة النقاط

**Example**

```
         shapeTextAlignment.setTopMarginPt(2.0d);
```

**Returns:**
double
### hashCode() {#hashCode--}
```
public int hashCode()
```




**Returns:**
int -
### isAutoMargin() {#isAutoMargin--}
```
public boolean isAutoMargin()
```


يشير إلى ما إذا كان هامش إطار النص تلقائيًا.

**Example**

```
         shapeTextAlignment.setAutoMargin(true);
```

**Returns:**
boolean
### isLockedText() {#isLockedText--}
```
public boolean isLockedText()
```


يشير إلى ما إذا كان الشكل مقفلًا عندما تكون ورقة العمل محمية.

**Remarks**

يعمل فقط عندما تكون ورقة العمل محمية.

**Returns:**
boolean
### isTextWrapped() {#isTextWrapped--}
```
public boolean isTextWrapped()
```


يحصل على نوع التفاف النص للشكل الذي يحتوي على نص.

**Example**

```
         shapeTextAlignment.setTextWrapped(true);
```

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




### setAutoMargin(boolean value) {#setAutoMargin-boolean-}
```
public void setAutoMargin(boolean value)
```


يشير إلى ما إذا كان هامش إطار النص تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAutoSize(boolean value) {#setAutoSize-boolean-}
```
public void setAutoSize(boolean value)
```


يشير إلى ما إذا كان حجم الشكل يتم ضبطه تلقائيًا وفقًا لمحتوياته.

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


يعيد الهامش الأيسر بوحدة النقاط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setLockedText(boolean value) {#setLockedText-boolean-}
```
public void setLockedText(boolean value)
```


يشير إلى ما إذا كان الشكل مقفلًا عندما تكون ورقة العمل محمية.

**Remarks**

يعمل فقط عندما تكون ورقة العمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setNumberOfColumns(int value) {#setNumberOfColumns-int-}
```
public void setNumberOfColumns(int value)
```


يضبط عدد أعمدة النص في المستطيل المحيط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRightMarginPt(double value) {#setRightMarginPt-double-}
```
public void setRightMarginPt(double value)
```


يعيد الهامش الأيمن بوحدة النقاط

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setRotateTextWithShape(boolean value) {#setRotateTextWithShape-boolean-}
```
public void setRotateTextWithShape(boolean value)
```


يشير إلى ما إذا كان النص يدور مع الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setRotationAngle(double value) {#setRotationAngle-double-}
```
public void setRotationAngle(double value)
```


يضبط دوران الشكل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setTextHorizontalOverflow(int value) {#setTextHorizontalOverflow-int-}
```
public void setTextHorizontalOverflow(int value)
```


يضبط نوع تجاوز النص الأفقي لصندوق النص.

انظر [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextShapeType(int value) {#setTextShapeType-int-}
```
public void setTextShapeType(int value)
```


يضبط نوع التحويل للنص.

انظر [AutoShapeType](../../com.aspose.cells/autoshapetype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextVerticalOverflow(int value) {#setTextVerticalOverflow-int-}
```
public void setTextVerticalOverflow(int value)
```


يضبط نوع تجاوز النص العمودي لصندوق النص.

انظر [TextOverflowType](../../com.aspose.cells/textoverflowtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextVerticalType(int value) {#setTextVerticalType-int-}
```
public void setTextVerticalType(int value)
```


يضبط اتجاه النص.

انظر [TextVerticalType](../../com.aspose.cells/textverticaltype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setTextWrapped(boolean value) {#setTextWrapped-boolean-}
```
public void setTextWrapped(boolean value)
```


يضبط نوع التفاف النص للشكل الذي يحتوي على نص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTopMarginPt(double value) {#setTopMarginPt-double-}
```
public void setTopMarginPt(double value)
```


يعيد الهامش العلوي بوحدة النقاط

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

