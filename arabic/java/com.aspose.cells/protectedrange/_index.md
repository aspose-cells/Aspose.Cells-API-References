---
title: "ProtectedRange"
second_title: "Aspose.Cells for Java API Reference"
description: "نطاق محدد يُسمح بتحريره عندما تكون حماية الورقة مفعلة."
type: docs
url: /ar/java/com.aspose.cells/protectedrange/
---

**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```

نطاق محدد يُسمح بتحريره عندما تكون حماية الورقة مفعلة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | يضيف مساحة مُشار إليها إلى هذا |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | يحصل على جميع المساحات المُشار إليها. |
| [getCellArea()](#getCellArea--) | يحصل على الكائن [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) الذي يمثل مساحة الخلية التي سيتم حمايتها. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | يحصل على عنوان النطاق. |
| [getPassword()](#getPassword--) | يمثل كلمة المرور لحماية النطاق. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | يحدد وصف الأمان حسابات المستخدمين الذين قد يحررون هذا النطاق دون تقديم كلمة مرور للوصول إلى النطاق. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | يشير إلى ما إذا كانت ورقة العمل محمية بكلمة مرور. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | يحصل على عنوان النطاق. |
| [setPassword(String value)](#setPassword-java.lang.String-) | يمثل كلمة المرور لحماية النطاق. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | يحدد وصف الأمان حسابات المستخدمين الذين قد يحررون هذا النطاق دون تقديم كلمة مرور للوصول إلى النطاق. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```


يضيف مساحة مُشار إليها إلى هذا

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية. |
| startColumn | int | عمود البداية. |
| endRow | int | صف النهاية. |
| endColumn | int | عمود النهاية. |

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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


يحصل على جميع المساحات المُشار إليها.

**Returns:**
com.aspose.cells.CellArea[] - يُرجع جميع المساحات المُشار إليها.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


يحصل على الكائن [getCellArea()](../../com.aspose.cells/protectedrange\#getCellArea--) الذي يمثل مساحة الخلية التي سيتم حمايتها.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```


يحصل على عنوان النطاق. يُستخدم هذا كواصف، وليس كتعريف نطاق مسمى.

**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```


يمثل كلمة المرور لحماية النطاق.

**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```


يحدد وصف الأمان حسابات المستخدمين الذين قد يحررون هذا النطاق دون تقديم كلمة مرور للوصول إلى النطاق.

**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```


يشير إلى ما إذا كانت ورقة العمل محمية بكلمة مرور.

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




### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يحصل على عنوان النطاق. يُستخدم هذا كواصف، وليس كتعريف نطاق مسمى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


يمثل كلمة المرور لحماية النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```


يحدد وصف الأمان حسابات المستخدمين الذين قد يحررون هذا النطاق دون تقديم كلمة مرور للوصول إلى النطاق.

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

