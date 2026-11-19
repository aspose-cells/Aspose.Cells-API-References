---
title: "ReferredArea"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل منطقة مُشار إليها بالصيغة."
type: docs
url: /ar/java/com.aspose.cells/referredarea/
---

**Inheritance:**
java.lang.Object
```
public class ReferredArea
```

يمثل منطقة مُشار إليها بالصيغة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getEndColumn()](#getEndColumn--) | عمود النهاية للمنطقة. |
| [getEndRow()](#getEndRow--) | صف النهاية للمنطقة. |
| [getExternalFileName()](#getExternalFileName--) | احصل على اسم الملف الخارجي إذا كان هذا إشارة خارجية. |
| [getSheetName()](#getSheetName--) | يشير إلى الورقة التي توجد فيها هذه الإشارة. |
| [getSheetNames()](#getSheetNames--) | أسماء جميع أوراق العمل التي تشير إليها هذه المثيلة. |
| [getStartColumn()](#getStartColumn--) | عمود البداية للمنطقة. |
| [getStartRow()](#getStartRow--) | صف البداية للمنطقة. |
| [getValue(int rowOffset, int colOffset)](#getValue-int-int-) | يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة. |
| [getValue(int rowOffset, int colOffset, boolean calculateFormulas)](#getValue-int-int-boolean-) | يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة. |
| [getValues()](#getValues--) | يحصل على قيم الخلايا في هذه المنطقة. |
| [getValues(boolean calculateFormulas)](#getValues-boolean-) | يحصل على قيم الخلايا في هذه المنطقة. |
| [hashCode()](#hashCode--) |  |
| [isArea()](#isArea--) | يشير إلى ما إذا كانت هذه منطقة. |
| [isEntireColumn()](#isEntireColumn--) | يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الصفوف(العمود بالكامل). |
| [isEntireRow()](#isEntireRow--) | يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الأعمدة(الصف بالكامل). |
| [isExternalLink()](#isExternalLink--) | يشير إلى ما إذا كان هذا رابطًا خارجيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) | يعيد عنوان المرجع لهذه المنطقة. |
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
### getEndColumn() {#getEndColumn--}
```
public int getEndColumn()
```


عمود النهاية للمنطقة.

**Returns:**
int
### getEndRow() {#getEndRow--}
```
public int getEndRow()
```


صف النهاية للمنطقة.

**Returns:**
int
### getExternalFileName() {#getExternalFileName--}
```
public String getExternalFileName()
```


احصل على اسم الملف الخارجي إذا كان هذا إشارة خارجية.

**Returns:**
java.lang.String
### getSheetName() {#getSheetName--}
```
public String getSheetName()
```


يشير إلى الورقة التي توجد فيها هذه الإشارة.

**Remarks**

إذا كان يشير إلى عدة أوراق عمل، فإن القيمة المرجعة تكون مثل تعبير النطاق في الصيغة. على سبيل المثال \"Sheet1:Sheet3\" للمرجع في الصيغة \"=SUM(Sheet1:Sheet3!$A$1:$B$2)\".

**Returns:**
java.lang.String
### getSheetNames() {#getSheetNames--}
```
public String[] getSheetNames()
```


أسماء جميع أوراق العمل التي تشير إليها هذه المثيلة.

**Returns:**
java.lang.String[]
### getStartColumn() {#getStartColumn--}
```
public int getStartColumn()
```


عمود البداية للمنطقة.

**Returns:**
int
### getStartRow() {#getStartRow--}
```
public int getStartRow()
```


صف البداية للمنطقة.

**Returns:**
int
### getValue(int rowOffset, int colOffset) {#getValue-int-int-}
```
public Object getValue(int rowOffset, int colOffset)
```


يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف من صف البداية لهذه المنطقة |
| colOffset | int | إزاحة العمود من صف البداية لهذه المنطقة |

**Returns:**
java.lang.Object - \"\\#REF!\" إذا كانت هذه المنطقة غير صالحة؛ \"\\#N/A\" إذا كان الإزاحة المعطاة خارج هذه المنطقة؛ وإلا يتم إرجاع قيمة الخلية في الموضع المعطى.
### getValue(int rowOffset, int colOffset, boolean calculateFormulas) {#getValue-int-int-boolean-}
```
public Object getValue(int rowOffset, int colOffset, boolean calculateFormulas)
```


يحصل على قيمة الخلية مع الإزاحة المحددة من أعلى اليسار لهذه المنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowOffset | int | إزاحة الصف من صف البداية لهذه المنطقة |
| colOffset | int | إزاحة العمود من صف البداية لهذه المنطقة |
| calculateFormulas | boolean | ما إذا كان يتم حسابه بشكل متكرر إذا كان المرجع المحدد صيغة |

**Returns:**
java.lang.Object - \"\\#REF!\" إذا كانت هذه المنطقة غير صالحة؛ \"\\#N/A\" إذا كان الإزاحة المعطاة خارج هذه المنطقة؛ وإلا يتم إرجاع قيمة الخلية في الموضع المعطى.
### getValues() {#getValues--}
```
public Object getValues()
```


يحصل على قيم الخلايا في هذه المنطقة.

**Returns:**
java.lang.Object - إذا كانت هذه المنطقة غير صالحة، سيتم إرجاع \"\\#REF!\"؛ إذا كانت هذه المنطقة خلية واحدة فقط، يتم إرجاع كائن قيمة الخلية؛ وإلا يتم إرجاع مصفوفة ثنائية الأبعاد لجميع القيم في هذه المنطقة.
### getValues(boolean calculateFormulas) {#getValues-boolean-}
```
public Object getValues(boolean calculateFormulas)
```


يحصل على قيم الخلايا في هذه المنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| calculateFormulas | boolean | في هذا النطاق، إذا كانت هناك بعض الصيغ التي لم تُحسب بعد، فإن هذه العلامة تشير إلى ما إذا كان يجب حساب تلك الصيغ بشكل متكرر |

**Returns:**
java.lang.Object - إذا كانت هذه المنطقة غير صالحة، سيتم إرجاع \"\\#REF!\"؛ إذا كانت هذه المنطقة خلية واحدة فقط، يتم إرجاع كائن قيمة الخلية؛ وإلا يتم إرجاع مصفوفة ثنائية الأبعاد لجميع القيم في هذه المنطقة.
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isArea() {#isArea--}
```
public boolean isArea()
```


يشير إلى ما إذا كانت هذه منطقة.

**Remarks**

إذا لم تكن هذه منطقة، فإن فقط StartRow وStartColumn لهما تأثير.

**Returns:**
boolean
### isEntireColumn() {#isEntireColumn--}
```
public boolean isEntireColumn()
```


يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الصفوف(العمود بالكامل).

**Returns:**
boolean
### isEntireRow() {#isEntireRow--}
```
public boolean isEntireRow()
```


يشير إلى ما إذا كانت هذه المنطقة تحتوي على جميع الأعمدة(الصف بالكامل).

**Returns:**
boolean
### isExternalLink() {#isExternalLink--}
```
public boolean isExternalLink()
```


يشير إلى ما إذا كان هذا رابطًا خارجيًا.

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




### toString() {#toString--}
```
public String toString()
```


يعيد عنوان المرجع لهذه المنطقة. عادةً ما يكون عنوان المرجع الذي يمكن استخدامه في الصيغة، مثل \"Sheet1!A1:C3\".

**Returns:**
java.lang.String - عنوان المرجع لهذه المنطقة.
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

