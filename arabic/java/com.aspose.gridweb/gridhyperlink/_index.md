---
title: "GridHyperlink"
second_title: "Aspose.Cells for Java API Reference"
description: "يحتوي على الكائن الذي يمثل ارتباطًا تشعبيًا."
type: docs
url: /ar/java/com.aspose.gridweb/gridhyperlink/
---

**Inheritance:**
java.lang.Object
```
public class GridHyperlink
```

يحتوي على الكائن الذي يمثل ارتباطًا تشعبيًا.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | يمثل عنوان الارتباط التشعبي. |
| [getAltText()](#getAltText--) | يحصل على النص البديل لرابط الصورة، يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel. |
| [getArea()](#getArea--) | يحصل على نطاق الارتباط التشعبي. |
| [getClass()](#getClass--) |  |
| [getCommand()](#getCommand--) | يرجع أو يضبط نص قيمة الأمر المعرّف ذاتيًا للرابط التشعبي المحدد. |
| [getDiscardInput()](#getDiscardInput--) | يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عند نقر المستخدم على هذا الرابط التشعبي CellCommand. |
| [getImageURL()](#getImageURL--) | يحصل على عنوان URL للصورة للرابط، لا توجد خاصية imageurl في الرابط التشعبي، لذا يتم في الواقع استخدام TextToDisplay لتسجيل هذه القيمة، سيتم تعيين TextToDisplay إلى <img src=value > وبالتالي سيتغير قيمة TextToDisplay. |
| [getScreenTip()](#getScreenTip--) | يعيد أو يحدد نص تلميح الشاشة للارتباط التشعبي المحدد. |
| [getTarget()](#getTarget--) | يحصل على نوع هدف الرابط الويب، يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel. |
| [getTextToDisplay()](#getTextToDisplay--) | يمثل النص الذي سيُعرض للارتباط التشعبي المحدد. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | يمثل عنوان الارتباط التشعبي. |
| [setAltText(String value)](#setAltText-java.lang.String-) | يضبط النص البديل لرابط الصورة، يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel. |
| [setCommand(String value)](#setCommand-java.lang.String-) | يرجع أو يضبط نص قيمة الأمر المعرّف ذاتيًا للرابط التشعبي المحدد. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عند نقر المستخدم على هذا الرابط التشعبي CellCommand. |
| [setImageURL(String value)](#setImageURL-java.lang.String-) | يضبط عنوان URL للصورة للرابط، لا توجد خاصية imageurl في الرابط التشعبي، لذا يتم في الواقع استخدام TextToDisplay لتسجيل هذه القيمة، سيتم تعيين TextToDisplay إلى <img src=value > وبالتالي سيتغير قيمة TextToDisplay. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | يعيد أو يحدد نص تلميح الشاشة للارتباط التشعبي المحدد. |
| [setTarget(String value)](#setTarget-java.lang.String-) | يضبط نوع هدف الرابط الويب، يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | يمثل النص الذي سيُعرض للارتباط التشعبي المحدد. |
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
### getAddress() {#getAddress--}
```
public String getAddress()
```


يمثل عنوان الارتباط التشعبي.

**Returns:**
java.lang.String
### getAltText() {#getAltText--}
```
public String getAltText()
```


يحصل على النص البديل لرابط الصورة، يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel.

**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public GridCellArea getArea()
```


يحصل على نطاق الارتباط التشعبي.

**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCommand() {#getCommand--}
```
public String getCommand()
```


يرجع أو يضبط نص قيمة الأمر المعرّف ذاتيًا للرابط التشعبي المحدد.

**Returns:**
java.lang.String
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```


يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عند نقر المستخدم على هذا الرابط التشعبي CellCommand. يمكن استخدامه كإجراء "undo" action.

**Returns:**
boolean
### getImageURL() {#getImageURL--}
```
public String getImageURL()
```


يحصل على عنوان URL للصورة للرابط، لا توجد خاصية imageurl في الرابط التشعبي، لذا يتم في الواقع استخدام TextToDisplay لتسجيل هذه القيمة، سيتم تعيين TextToDisplay إلى <img src=value > وبالتالي سيتغير قيمة TextToDisplay.

**Returns:**
java.lang.String
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```


يعيد أو يحدد نص تلميح الشاشة للارتباط التشعبي المحدد.

**Returns:**
java.lang.String
### getTarget() {#getTarget--}
```
public String getTarget()
```


يحصل على نوع هدف الرابط الويب، يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel.

**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```


يمثل النص الذي سيُعرض للارتباط التشعبي المحدد. القيمة الافتراضية هي عنوان الارتباط التشعبي.

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




### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```


يمثل عنوان الارتباط التشعبي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAltText(String value) {#setAltText-java.lang.String-}
```
public void setAltText(String value)
```


يضبط النص البديل لرابط الصورة، يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```


يرجع أو يضبط نص قيمة الأمر المعرّف ذاتيًا للرابط التشعبي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```


يشير إلى ما إذا كان يجب تجاهل إدخال المستخدم في متصفح العميل عند نقر المستخدم على هذا الرابط التشعبي CellCommand. يمكن استخدامه كإجراء "undo" action.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setImageURL(String value) {#setImageURL-java.lang.String-}
```
public void setImageURL(String value)
```


يضبط عنوان URL للصورة للرابط، لا توجد خاصية imageurl في الرابط التشعبي، لذا يتم في الواقع استخدام TextToDisplay لتسجيل هذه القيمة، سيتم تعيين TextToDisplay إلى <img src=value > وبالتالي سيتغير قيمة TextToDisplay.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```


يعيد أو يحدد نص تلميح الشاشة للارتباط التشعبي المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTarget(String value) {#setTarget-java.lang.String-}
```
public void setTarget(String value)
```


يضبط نوع هدف الرابط الويب، يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```


يمثل النص الذي سيُعرض للارتباط التشعبي المحدد. القيمة الافتراضية هي عنوان الارتباط التشعبي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

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

