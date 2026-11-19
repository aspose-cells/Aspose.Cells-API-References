---
title: "PivotCache"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل ذاكرة التخزين المؤقت لبعض تقارير جدول المحور."
type: docs
url: /ar/java/com.aspose.cells/pivotcache/
---

**Inheritance:**
java.lang.Object
```
public abstract class PivotCache
```

يمثل ذاكرة التخزين المؤقت لبعض تقارير جدول المحور.

**Remarks**

سيتم جمع جميع البيانات في هذه الذاكرة المؤقتة، وستحصل الجداول المحورية على البيانات فقط من هذه الذاكرة المؤقتة، دون الوصول مباشرة إلى مصدر البيانات. إذا كان مصدر البيانات لبعض [PivotTable](../../com.aspose.cells/pivottable)s هو نفسه، فستستخدم ذاكرة مؤقتة محورية.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [PivotCache()](#PivotCache--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [dispose()](#dispose--) | إطلاق جميع الموارد. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getMissingItemsLimit()](#getMissingItemsLimit--) | يحصل على عدد العناصر غير المستخدمة المسموح بها قبل حذف العناصر غير المستخدمة. |
| [getPivotTables()](#getPivotTables--) | يحصل على جميع الجداول المحورية التي تستخدم هذه الذاكرة المؤقتة. |
| [getSourceType()](#getSourceType--) | يحصل على [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype). |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات للعرض الخاص بجميع الجداول المحورية التي يكون مصدر بياناتها هذه الذاكرة المؤقتة. |
| [refresh(PivotTableRefreshOption option)](#refresh-com.aspose.cells.PivotTableRefreshOption-) | يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات للعرض الخاص بجميع الجداول المحورية التي يكون مصدر بياناتها هذه الذاكرة المؤقتة. |
| [setMissingItemsLimit(int value)](#setMissingItemsLimit-int-) | يضبط عدد العناصر غير المستخدمة المسموح بها قبل حذف العناصر غير المستخدمة. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### PivotCache() {#PivotCache--}
```
public PivotCache()
```


### dispose() {#dispose--}
```
public abstract void dispose()
```


إطلاق جميع الموارد.

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
### getMissingItemsLimit() {#getMissingItemsLimit--}
```
public int getMissingItemsLimit()
```


يحصل على عدد العناصر غير المستخدمة المسموح بها قبل حذف العناصر غير المستخدمة. يجب أن تكون هذه القيمة أكبر من -2 وأقل من 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

**Returns:**
int
### getPivotTables() {#getPivotTables--}
```
public PivotTable[] getPivotTables()
```


يحصل على جميع الجداول المحورية التي تستخدم هذه الذاكرة المؤقتة.

**Returns:**
com.aspose.cells.PivotTable[] -
### getSourceType() {#getSourceType--}
```
public abstract byte getSourceType()
```


يحصل على [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

انظر [PivotTableSourceType](../../com.aspose.cells/pivottablesourcetype).

**Returns:**
byte
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




### refresh() {#refresh--}
```
public int refresh()
```


يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات للعرض الخاص بجميع الجداول المحورية التي يكون مصدر بياناتها هذه الذاكرة المؤقتة.

**Remarks**

إذا كان كل من table1 و table2 يستخدمان هذه الذاكرة المؤقتة، سيتم حساب الجدولين. من الأفضل أن تقوم ببساطة باستدعاء [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) لتحديث جميع الجداول المحورية والمخططات في الملف.

**Returns:**
int
### refresh(PivotTableRefreshOption option) {#refresh-com.aspose.cells.PivotTableRefreshOption-}
```
public int refresh(PivotTableRefreshOption option)
```


يقوم بتحديث البيانات من مصدر البيانات ويحسب البيانات للعرض الخاص بجميع الجداول المحورية التي يكون مصدر بياناتها هذه الذاكرة المؤقتة.

**Remarks**

من الأفضل أن تقوم ببساطة باستدعاء [Workbook.refreshAll()](../../com.aspose.cells/workbook\#refreshAll--) لتحديث جميع الجداول المحورية والمخططات في الملف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| option | [PivotTableRefreshOption](../../com.aspose.cells/pivottablerefreshoption) | الخيارات لتحديث مصدر بيانات الجدول المحوري. |

**Returns:**
int
### setMissingItemsLimit(int value) {#setMissingItemsLimit-int-}
```
public void setMissingItemsLimit(int value)
```


يضبط عدد العناصر غير المستخدمة المسموح بها قبل حذف العناصر غير المستخدمة. يجب أن تكون هذه القيمة أكبر من -2 وأقل من 1048577. [PivotCacheMissingItemsLimitConst](../../com.aspose.cells/pivotcachemissingitemslimitconst);

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

