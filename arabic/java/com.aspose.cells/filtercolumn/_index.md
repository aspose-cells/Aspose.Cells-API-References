---
title: "FilterColumn"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل فلترًا لعمود واحد أو عمود في الجدول."
type: docs
url: /ar/java/com.aspose.cells/filtercolumn/
---

**Inheritance:**
java.lang.Object
```
public class FilterColumn
```

يمثل فلترًا لعمود واحد أو عمود في الجدول.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColorFilter()](#getColorFilter--) | يحصل على [ColorFilter](../../com.aspose.cells/colorfilter) لتصفية البيانات حسب اللون. |
| [getCustomFilters()](#getCustomFilters--) | يحصل على [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) لتصفية البيانات وفق معايير مخصصة. |
| [getDynamicFilter()](#getDynamicFilter--) | يحصل على [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) لتصفية باستخدام معايير ديناميكية. |
| [getFieldIndex()](#getFieldIndex--) | يحصل على إزاحة العمود في النطاق. |
| [getFilter()](#getFilter--) | يحصل على شرط تصفية البيانات. |
| [getFilterType()](#getFilterType--) | يحصل على نوع تصفية البيانات. |
| [getFilterValues()](#getFilterValues--) | يحصل على [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) لتصفية البيانات حسب التسميات أو التاريخ والوقت. |
| [getIconFilter()](#getIconFilter--) | يحصل على [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) لتصفية البيانات حسب الأيقونة. |
| [getMultipleFilters()](#getMultipleFilters--) | يحصل على [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) لتصفية البيانات حسب التسميات أو التاريخ والوقت. |
| [getTop10Filter()](#getTop10Filter--) | يحصل على [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) لتصفية البيانات حسب ترتيب البيانات. |
| [hashCode()](#hashCode--) |  |
| [isDropdownVisible()](#isDropdownVisible--) | يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [selectAll()](#selectAll--) | يحدد الكل. |
| [setCustomFilters(CustomFilterCollection value)](#setCustomFilters-com.aspose.cells.CustomFilterCollection-) | يحصل على [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) لتصفية البيانات وفق معايير مخصصة. |
| [setDropdownVisible(boolean value)](#setDropdownVisible-boolean-) | يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا. |
| [setFieldIndex(int value)](#setFieldIndex-int-) | يضبط إزاحة العمود في النطاق. |
| [setFilter(Object value)](#setFilter-java.lang.Object-) | يضبط شرط تصفية البيانات. |
| [setFilterType(int value)](#setFilterType-int-) | يضبط نوع تصفية البيانات. |
| [setMultipleFilters(MultipleFilterCollection value)](#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-) | يحصل على [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) لتصفية البيانات حسب التسميات أو التاريخ والوقت. |
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
### getColorFilter() {#getColorFilter--}
```
public ColorFilter getColorFilter()
```


يحصل على [ColorFilter](../../com.aspose.cells/colorfilter) لتصفية البيانات حسب اللون.

**Remarks**

يضبط [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) كـ [FilterType.COLOR\_FILTER](../../com.aspose.cells/filtertype\#COLOR-FILTER) أولاً، وإلا سيتم إرجاع Null.

**Returns:**
[ColorFilter](../../com.aspose.cells/colorfilter)
### getCustomFilters() {#getCustomFilters--}
```
public CustomFilterCollection getCustomFilters()
```


يحصل على [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) لتصفية البيانات وفق معايير مخصصة.

**Remarks**

ملاحظة: هذه الدالة الضابطة لهذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) عن طريق ضبطها كـ [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[CustomFilterCollection](../../com.aspose.cells/customfiltercollection)
### getDynamicFilter() {#getDynamicFilter--}
```
public DynamicFilter getDynamicFilter()
```


يحصل على [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) لتصفية باستخدام معايير ديناميكية.

**Remarks**

قبل استخدام هذه الخاصية، يرجى التأكد من أن [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) هو [FilterType.DYNAMIC\_FILTER](../../com.aspose.cells/filtertype\#DYNAMIC-FILTER)، وإلا سيتم إرجاع null.

**Returns:**
[DynamicFilter](../../com.aspose.cells/dynamicfilter)
### getFieldIndex() {#getFieldIndex--}
```
public int getFieldIndex()
```


يحصل على إزاحة العمود في النطاق.

**Returns:**
int
### getFilter() {#getFilter--}
```
public Object getFilter()
```


يحصل على شرط تصفية البيانات.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية المقابلة وفقًا لـ [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). ولنوع الفلتر [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS)، الكائن المرتجع هو الآن [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) بدلاً من [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
java.lang.Object
### getFilterType() {#getFilterType--}
```
public int getFilterType()
```


يحصل على نوع تصفية البيانات.

انظر إلى [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

سيتم إنشاء كائن الفلتر المقابل عند ضبط هذه الخاصية ويجب استخدام الخاصية المقابلة للحصول على كائن الفلتر وفقًا لذلك:

| FilterType | خاصية |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Returns:**
int
### getFilterValues() {#getFilterValues--}
```
public FilterValueCollection getFilterValues()
```


يحصل على [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) لتصفية البيانات حسب التسميات أو التاريخ والوقت.

**Remarks**

يضبط [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) كـ [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS) أولاً، وإلا سيتم إرجاع Null.

**Returns:**
[FilterValueCollection](../../com.aspose.cells/filtervaluecollection)
### getIconFilter() {#getIconFilter--}
```
public IconFilter getIconFilter()
```


يحصل على [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) لتصفية البيانات حسب الأيقونة.

**Remarks**

قبل استخدام هذه الخاصية، يرجى التأكد من أن [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) هو [FilterType.ICON\_FILTER](../../com.aspose.cells/filtertype\#ICON-FILTER)، وإلا سيتم إرجاع null.

**Returns:**
[IconFilter](../../com.aspose.cells/iconfilter)
### getMultipleFilters() {#getMultipleFilters--}
```
public MultipleFilterCollection getMultipleFilters()
```


يحصل على [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) لتصفية البيانات حسب التسميات أو التاريخ والوقت.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية FilterColumn.FilterValues. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Returns:**
[MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection)
### getTop10Filter() {#getTop10Filter--}
```
public Top10Filter getTop10Filter()
```


يحصل على [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) لتصفية البيانات حسب ترتيب البيانات.

**Remarks**

قبل استخدام هذه الخاصية، يرجى التأكد من أن [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) هو [FilterType.TOP\_10](../../com.aspose.cells/filtertype\#TOP-10)، وإلا سيتم إرجاع null.

**Returns:**
[Top10Filter](../../com.aspose.cells/top10filter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isDropdownVisible() {#isDropdownVisible--}
```
public boolean isDropdownVisible()
```


يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا.

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




### selectAll() {#selectAll--}
```
public void selectAll()
```


يحدد الكل.

### setCustomFilters(CustomFilterCollection value) {#setCustomFilters-com.aspose.cells.CustomFilterCollection-}
```
public void setCustomFilters(CustomFilterCollection value)
```


يحصل على [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) لتصفية البيانات وفق معايير مخصصة.

**Remarks**

ملاحظة: هذه الدالة الضابطة لهذه الخاصية أصبحت الآن مهجورة. بدلاً من ذلك، يرجى استخدام الخاصية [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--) عن طريق ضبطها كـ [FilterType.CUSTOM\_FILTERS](../../com.aspose.cells/filtertype\#CUSTOM-FILTERS). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [CustomFilterCollection](../../com.aspose.cells/customfiltercollection) |  |

### setDropdownVisible(boolean value) {#setDropdownVisible-boolean-}
```
public void setDropdownVisible(boolean value)
```


يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setFieldIndex(int value) {#setFieldIndex-int-}
```
public void setFieldIndex(int value)
```


يضبط إزاحة العمود في النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFilter(Object value) {#setFilter-java.lang.Object-}
```
public void setFilter(Object value)
```


يضبط شرط تصفية البيانات.

**Remarks**

ملاحظة: هذا العضو أصبح الآن مهجورًا. بدلاً من ذلك، يرجى استخدام الخاصية المقابلة وفقًا لـ [getFilterType()](../../com.aspose.cells/filtercolumn\#getFilterType--). ولنوع الفلتر [FilterType.MULTIPLE\_FILTERS](../../com.aspose.cells/filtertype\#MULTIPLE-FILTERS)، الكائن المرتجع هو الآن [FilterValueCollection](../../com.aspose.cells/filtervaluecollection) بدلاً من [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection). سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ أكتوبر 2025. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### setFilterType(int value) {#setFilterType-int-}
```
public void setFilterType(int value)
```


يضبط نوع تصفية البيانات.

انظر إلى [FilterType](../../com.aspose.cells/filtertype).

**Remarks**

سيتم إنشاء كائن الفلتر المقابل عند ضبط هذه الخاصية ويجب استخدام الخاصية المقابلة للحصول على كائن الفلتر وفقًا لذلك:

| FilterType | خاصية |
| --------------- | ---------------------------------------------------------------------------- |
| MultipleFilters | [getFilterValues()](../../com.aspose.cells/filtercolumn\#getFilterValues--) |
| CustomFilters | [getCustomFilters()](../../com.aspose.cells/filtercolumn\#getCustomFilters--) |
| ColorFilter | [getColorFilter()](../../com.aspose.cells/filtercolumn\#getColorFilter--) |
| DynamicFilter | [getDynamicFilter()](../../com.aspose.cells/filtercolumn\#getDynamicFilter--) |
| IconFilter | [getIconFilter()](../../com.aspose.cells/filtercolumn\#getIconFilter--) |
| Top10 | [getTop10Filter()](../../com.aspose.cells/filtercolumn\#getTop10Filter--) |

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setMultipleFilters(MultipleFilterCollection value) {#setMultipleFilters-com.aspose.cells.MultipleFilterCollection-}
```
public void setMultipleFilters(MultipleFilterCollection value)
```


يحصل على [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) لتصفية البيانات حسب التسميات أو التاريخ والوقت.

**Remarks**

ملاحظة: هذا العضو أصبح الآن غير صالح. بدلاً من ذلك، يرجى استخدام خاصية FilterColumn.FilterValues. سيتم إزالة هذه الخاصية بعد 12 شهرًا منذ يونيو 2026. تعتذر Aspose عن أي إزعاج قد تكون قد واجهته.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [MultipleFilterCollection](../../com.aspose.cells/multiplefiltercollection) |  |

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

