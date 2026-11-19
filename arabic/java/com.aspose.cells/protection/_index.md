---
title: "الحماية"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الأنواع المختلفة لخيارات الحماية المتاحة لورقة العمل."
type: docs
url: /ar/java/com.aspose.cells/protection/
---

**Inheritance:**
java.lang.Object
```
public class Protection
```

يمثل الأنواع المختلفة لخيارات الحماية المتاحة لورقة العمل.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
 
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Allowing users to select locked cells of the worksheet
         worksheet.getProtection().setAllowSelectingLockedCell(true);
         //Allowing users to select unlocked cells of the worksheet
         worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | نسخ معلومات الحماية. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | يمثل ما إذا كان حذف الأعمدة مسموحًا به في ورقة عمل محمية. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | يمثل ما إذا كان حذف الصفوف مسموحًا به في ورقة عمل محمية. |
| [getAllowEditingContent()](#getAllowEditingContent--) | يمثل ما إذا كان المستخدم مسموحًا له بتحرير محتويات الخلايا المقفلة في ورقة عمل محمية. |
| [getAllowEditingObject()](#getAllowEditingObject--) | يمثل ما إذا كان المستخدم مسموحًا له بالتعامل مع كائنات الرسم في ورقة عمل محمية. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | يمثل ما إذا كان المستخدم مسموحًا له بتحرير السيناريوهات في ورقة عمل محمية. |
| [getAllowFiltering()](#getAllowFiltering--) | يمثل ما إذا كان المستخدم مسموحًا له باستخدام AutoFilter الذي تم إنشاؤه قبل حماية الورقة. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | يمثل ما إذا كان تنسيق الخلايا مسموحًا به في ورقة عمل محمية. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | يمثل ما إذا كان تنسيق الأعمدة مسموحًا به في ورقة عمل محمية. |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | يمثل ما إذا كان تنسيق الصفوف مسموحًا به في ورقة عمل محمية. |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | يمثل ما إذا كان إدراج الأعمدة مسموحًا به في ورقة عمل محمية |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | يمثل ما إذا كان إدراج الروابط التشعبية مسموحًا به في ورقة عمل محمية |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | يمثل ما إذا كان إدراج الصفوف مسموحًا به في ورقة عمل محمية |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا المقفلة في ورقة عمل محمية. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا غير المقفلة في ورقة عمل محمية. |
| [getAllowSorting()](#getAllowSorting--) | يمثل ما إذا كان خيار الفرز مسموحًا به في ورقة عمل محمية. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | يمثل ما إذا كان يُسمح للمستخدم بالتعامل مع جداول المحور في ورقة عمل محمية. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | يمثل كلمة المرور لحماية ورقة العمل. |
| [getPasswordHash()](#getPasswordHash--) | يحصل على التجزئة لكلمة المرور الحالية. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | يشير إلى ما إذا كانت ورقة العمل محمية بكلمة مرور. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | يمثل ما إذا كان حذف الأعمدة مسموحًا به في ورقة عمل محمية. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | يمثل ما إذا كان حذف الصفوف مسموحًا به في ورقة عمل محمية. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | يمثل ما إذا كان المستخدم مسموحًا له بتحرير محتويات الخلايا المقفلة في ورقة عمل محمية. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | يمثل ما إذا كان المستخدم مسموحًا له بالتعامل مع كائنات الرسم في ورقة عمل محمية. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | يمثل ما إذا كان المستخدم مسموحًا له بتحرير السيناريوهات في ورقة عمل محمية. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | يمثل ما إذا كان المستخدم مسموحًا له باستخدام AutoFilter الذي تم إنشاؤه قبل حماية الورقة. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | يمثل ما إذا كان تنسيق الخلايا مسموحًا به في ورقة عمل محمية. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | يمثل ما إذا كان تنسيق الأعمدة مسموحًا به في ورقة عمل محمية. |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | يمثل ما إذا كان تنسيق الصفوف مسموحًا به في ورقة عمل محمية. |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | يمثل ما إذا كان إدراج الأعمدة مسموحًا به في ورقة عمل محمية |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | يمثل ما إذا كان إدراج الروابط التشعبية مسموحًا به في ورقة عمل محمية |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | يمثل ما إذا كان إدراج الصفوف مسموحًا به في ورقة عمل محمية |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا المقفلة في ورقة عمل محمية. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا غير المقفلة في ورقة عمل محمية. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | يمثل ما إذا كان خيار الفرز مسموحًا به في ورقة عمل محمية. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | يمثل ما إذا كان يُسمح للمستخدم بالتعامل مع جداول المحور في ورقة عمل محمية. |
| [setPassword(String value)](#setPassword-java.lang.String-) | يمثل كلمة المرور لحماية ورقة العمل. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | يتحقق من كلمة المرور. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```


نسخ معلومات الحماية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |

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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```


يمثل ما إذا كان حذف الأعمدة مسموحًا به في ورقة عمل محمية.

**Remarks**

يجب أن تكون الأعمدة التي تحتوي على الخلايا المراد حذفها غير مقفلة عندما تكون الورقة محمية، ويجب تمكين خيار "Select unlocked cells".

**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```


يمثل ما إذا كان حذف الصفوف مسموحًا به في ورقة عمل محمية.

**Remarks**

يجب أن تكون الصفوف التي تحتوي على الخلايا المراد حذفها غير مقفلة عندما تكون الورقة محمية، ويجب تمكين خيار "Select unlocked cells".

**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```


يمثل ما إذا كان المستخدم مسموحًا له بتحرير محتويات الخلايا المقفلة في ورقة عمل محمية.

**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```


يمثل ما إذا كان المستخدم مسموحًا له بالتعامل مع كائنات الرسم في ورقة عمل محمية.

**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```


يمثل ما إذا كان المستخدم مسموحًا له بتحرير السيناريوهات في ورقة عمل محمية.

**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```


يمثل ما إذا كان المستخدم مسموحًا له باستخدام AutoFilter الذي تم إنشاؤه قبل حماية الورقة.

**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```


يمثل ما إذا كان تنسيق الخلايا مسموحًا به في ورقة عمل محمية.

**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```


يمثل ما إذا كان تنسيق الأعمدة مسموحًا به في ورقة عمل محمية.

**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```


يمثل ما إذا كان تنسيق الصفوف مسموحًا به في ورقة عمل محمية.

**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```


يمثل ما إذا كان إدراج الأعمدة مسموحًا به في ورقة عمل محمية

**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```


يمثل ما إذا كان إدراج الروابط التشعبية مسموحًا به في ورقة عمل محمية

**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```


يمثل ما إذا كان إدراج الصفوف مسموحًا به في ورقة عمل محمية

**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```


يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا المقفلة في ورقة عمل محمية.

**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```


يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا غير المقفلة في ورقة عمل محمية.

**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```


يمثل ما إذا كان خيار الفرز مسموحًا به في ورقة عمل محمية.

**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```


يمثل ما إذا كان يُسمح للمستخدم بالتعامل مع جداول المحور في ورقة عمل محمية.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```


يمثل كلمة المرور لحماية ورقة العمل.

**Remarks**

إذا تم تعيين كلمة المرور إلى null أو سلسلة فارغة، يمكنك إلغاء حماية ورقة العمل أو المصنف دون استخدام كلمة مرور. وإلا، يجب عليك تحديد كلمة المرور لإلغاء حماية ورقة العمل أو المصنف.

**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```


يحصل على التجزئة لكلمة المرور الحالية.

**Returns:**
int
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




### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```


يمثل ما إذا كان حذف الأعمدة مسموحًا به في ورقة عمل محمية.

**Remarks**

يجب أن تكون الأعمدة التي تحتوي على الخلايا المراد حذفها غير مقفلة عندما تكون الورقة محمية، ويجب تمكين خيار "Select unlocked cells".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```


يمثل ما إذا كان حذف الصفوف مسموحًا به في ورقة عمل محمية.

**Remarks**

يجب أن تكون الصفوف التي تحتوي على الخلايا المراد حذفها غير مقفلة عندما تكون الورقة محمية، ويجب تمكين خيار "Select unlocked cells".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```


يمثل ما إذا كان المستخدم مسموحًا له بتحرير محتويات الخلايا المقفلة في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```


يمثل ما إذا كان المستخدم مسموحًا له بالتعامل مع كائنات الرسم في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```


يمثل ما إذا كان المستخدم مسموحًا له بتحرير السيناريوهات في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```


يمثل ما إذا كان المستخدم مسموحًا له باستخدام AutoFilter الذي تم إنشاؤه قبل حماية الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```


يمثل ما إذا كان تنسيق الخلايا مسموحًا به في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```


يمثل ما إذا كان تنسيق الأعمدة مسموحًا به في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```


يمثل ما إذا كان تنسيق الصفوف مسموحًا به في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```


يمثل ما إذا كان إدراج الأعمدة مسموحًا به في ورقة عمل محمية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```


يمثل ما إذا كان إدراج الروابط التشعبية مسموحًا به في ورقة عمل محمية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```


يمثل ما إذا كان إدراج الصفوف مسموحًا به في ورقة عمل محمية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```


يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا المقفلة في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```


يمثل ما إذا كان يُسمح للمستخدم بتحديد الخلايا غير المقفلة في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```


يمثل ما إذا كان خيار الفرز مسموحًا به في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```


يمثل ما إذا كان يُسمح للمستخدم بالتعامل مع جداول المحور في ورقة عمل محمية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```


يمثل كلمة المرور لحماية ورقة العمل.

**Remarks**

إذا تم تعيين كلمة المرور إلى null أو سلسلة فارغة، يمكنك إلغاء حماية ورقة العمل أو المصنف دون استخدام كلمة مرور. وإلا، يجب عليك تحديد كلمة المرور لإلغاء حماية ورقة العمل أو المصنف.

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
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```


يتحقق من كلمة المرور.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| password | java.lang.String | كلمة المرور. |

**Returns:**
boolean -
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

