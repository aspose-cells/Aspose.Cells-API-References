---
title: "AutoFilter"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل الترشيح التلقائي للورقة المحددة."
type: docs
url: /ar/java/com.aspose.cells/autofilter/
---

**Inheritance:**
java.lang.Object
```
public class AutoFilter
```

يمثل الترشيح التلقائي للورقة المحددة.

**Example**

```
         //Creating a file stream containing the Excel file to be opened
         //Instantiating a Workbook object
         Workbook workbook = new Workbook("template.xlsx");
         //Accessing the first worksheet in the Excel file
         Worksheet worksheet = workbook.getWorksheets().get(0);
         //Creating AutoFilter by giving the cells range of the heading row
         worksheet.getAutoFilter().setRange("A1:B1");
         //Filtering columns with specified values
         worksheet.getAutoFilter().filter(1, "Bananas");
         //Saving the modified Excel file.
         workbook.save("output.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#addDateFilter-int-int-int-int-int-int-int-int-) | يضيف مرشح تاريخ. |
| [addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)](#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-) | يضيف مرشح لون تعبئة. |
| [addFilter(int fieldIndex, String criteria)](#addFilter-int-java.lang.String-) | يضيف مرشحًا لعمود الفلترة. |
| [addFontColorFilter(int fieldIndex, CellsColor color)](#addFontColorFilter-int-com.aspose.cells.CellsColor-) | يضيف مرشح لون الخط. |
| [addIconFilter(int fieldIndex, int iconSetType, int iconId)](#addIconFilter-int-int-int-) | يضيف مرشح أيقونة. |
| [custom(int fieldIndex, int operatorType1, Object criteria1)](#custom-int-int-java.lang.Object-) | يفلتر قائمة باستخدام معيار مخصص. |
| [custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)](#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-) | يفلتر قائمة باستخدام معايير مخصصة. |
| [dynamicFilter(int fieldIndex, int dynamicFilterType)](#dynamicFilter-int-int-) | يضيف مرشحًا ديناميكيًا. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filter(int fieldIndex, String criteria)](#filter-int-java.lang.String-) | يفلتر قائمة باستخدام معايير محددة. |
| [filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)](#filterTop10-int-boolean-boolean-int-) | تصفية أعلى 10 عناصر في القائمة |
| [getCellArea()](#getCellArea--) | يحصل على [CellArea](../../com.aspose.cells/cellarea) حيث ينطبق هذا AutoFilter. |
| [getCellArea(boolean refreshAppliedRange)](#getCellArea-boolean-) | يحصل على [CellArea](../../com.aspose.cells/cellarea) حيث ينطبق AutoFilter المحدد. |
| [getClass()](#getClass--) |  |
| [getFilterColumns()](#getFilterColumns--) | يحصل على مجموعة أعمدة الفلترة. |
| [getRange()](#getRange--) | يمثل النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [getShowFilterButton()](#getShowFilterButton--) | يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا. |
| [getSorter()](#getSorter--) | يحصل على مُرتب البيانات. |
| [hashCode()](#hashCode--) |  |
| [matchBlanks(int fieldIndex)](#matchBlanks-int-) | مطابقة جميع الخلايا الفارغة في القائمة. |
| [matchNonBlanks(int fieldIndex)](#matchNonBlanks-int-) | مطابقة جميع الخلايا غير الفارغة في القائمة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refresh()](#refresh--) | تحديث الفلاتر التلقائية لإخفاء أو إظهار الصفوف. |
| [refresh(boolean hideRows)](#refresh-boolean-) | يحصل على مؤشرات جميع الصفوف المخفية. |
| [removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)](#removeDateFilter-int-int-int-int-int-int-int-int-) | يزيل مرشح التاريخ. |
| [removeFilter(int fieldIndex)](#removeFilter-int-) | يزيل المرشح المحدد. |
| [removeFilter(int fieldIndex, String criteria)](#removeFilter-int-java.lang.String-) | يزيل مرشحًا لعمود الفلترة. |
| [setRange(int row, int startColumn, int endColumn)](#setRange-int-int-int-) | يضبط النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [setRange(String value)](#setRange-java.lang.String-) | يمثل النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [setShowFilterButton(boolean value)](#setShowFilterButton-boolean-) | يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا. |
| [showAll()](#showAll--) | إظهار جميع الصفوف. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#addDateFilter-int-int-int-int-int-int-int-int-}
```
public void addDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


يضيف مرشح تاريخ.

**Remarks**

إذا كان DateTimeGroupingType هو Year، فإن المعامل year فقط هو الفعّال. إذا كان DateTiemGroupingType هو Month، فإن المعاملين year و month فقط هما الفعّالان.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). نوع التجميع |
| سنة | int | السنة. |
| شهر | int | الشهر. |
| يوم | int | اليوم. |
| ساعة | int | الساعة. |
| دقيقة | int | الدقيقة. |
| ثانية | int | الثانية. |

### addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor) {#addFillColorFilter-int-int-com.aspose.cells.CellsColor-com.aspose.cells.CellsColor-}
```
public void addFillColorFilter(int fieldIndex, int pattern, CellsColor foregroundColor, CellsColor backgroundColor)
```


يضيف مرشح لون تعبئة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| pattern | int | [BackgroundType](../../com.aspose.cells/backgroundtype). نوع نمط الخلفية |
| foregroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | لون المقدمة. |
| backgroundColor | [CellsColor](../../com.aspose.cells/cellscolor) | لون الخلفية. |

### addFilter(int fieldIndex, String criteria) {#addFilter-int-java.lang.String-}
```
public void addFilter(int fieldIndex, String criteria)
```


يضيف مرشحًا لعمود الفلترة.

**Remarks**

يدعم MS Excel 2007 اختيارًا متعددًا في عمود الفلتر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| معايير | java.lang.String | المعيار المحدد (سلسلة؛ على سبيل المثال، \"101\"). يمكن أن يكون إما فارغًا أو أحد قيم الخلايا في هذا العمود. |

### addFontColorFilter(int fieldIndex, CellsColor color) {#addFontColorFilter-int-com.aspose.cells.CellsColor-}
```
public void addFontColorFilter(int fieldIndex, CellsColor color)
```


يضيف مرشح لون الخط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| color | [CellsColor](../../com.aspose.cells/cellscolor) | كائن [CellsColor](../../com.aspose.cells/cellscolor). |

### addIconFilter(int fieldIndex, int iconSetType, int iconId) {#addIconFilter-int-int-int-}
```
public void addIconFilter(int fieldIndex, int iconSetType, int iconId)
```


يضيف مرشح أيقونة.

**Remarks**

يدعم فقط إضافة مرشح الأيقونة. لا يدعم التحقق من أي صف ظاهر إذا كان المرشح هو مرشح الأيقونة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| iconSetType | int | [IconSetType](../../com.aspose.cells/iconsettype). نوع مجموعة الأيقونات |
| iconId | int | معرف الأيقونة. |

### custom(int fieldIndex, int operatorType1, Object criteria1) {#custom-int-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1)
```


يفلتر قائمة باستخدام معيار مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). نوع عامل الفلتر |
| criteria1 | java.lang.Object | المعيار المخصص |

### custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2) {#custom-int-int-java.lang.Object-boolean-int-java.lang.Object-}
```
public void custom(int fieldIndex, int operatorType1, Object criteria1, boolean isAnd, int operatorType2, Object criteria2)
```


يفلتر قائمة باستخدام معايير مخصصة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| operatorType1 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). نوع عامل الفلتر |
| criteria1 | java.lang.Object | المعيار المخصص |
| isAnd | boolean |  |
| operatorType2 | int | [FilterOperatorType](../../com.aspose.cells/filteroperatortype). نوع عامل الفلتر |
| criteria2 | java.lang.Object | المعيار المخصص |

### dynamicFilter(int fieldIndex, int dynamicFilterType) {#dynamicFilter-int-int-}
```
public void dynamicFilter(int fieldIndex, int dynamicFilterType)
```


يضيف مرشحًا ديناميكيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| dynamicFilterType | int | [DynamicFilterType](../../com.aspose.cells/dynamicfiltertype). نوع الفلتر الديناميكي. |

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
### filter(int fieldIndex, String criteria) {#filter-int-java.lang.String-}
```
public void filter(int fieldIndex, String criteria)
```


يفلتر قائمة باستخدام معايير محددة.

**Remarks**

Aspose.Cells ستزيل جميع إعدادات الفلاتر الأخرى في هذا الحقل كما في MS Excel 97-2003.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| معايير | java.lang.String | المعيار المحدد (سلسلة؛ على سبيل المثال، "101"). |

### filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount) {#filterTop10-int-boolean-boolean-int-}
```
public void filterTop10(int fieldIndex, boolean isTop, boolean isPercent, int itemCount)
```


تصفية أعلى 10 عناصر في القائمة

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| isTop | boolean | يشير إلى ما إذا كان الفلتر من الأعلى أو الأسفل |
| isPercent | boolean | يشير إلى ما إذا كان العنصر نسبة مئوية أم عدد |
| itemCount | int | عدد العناصر |

### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```


يحصل على [CellArea](../../com.aspose.cells/cellarea) حيث ينطبق هذا AutoFilter.

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getCellArea(boolean refreshAppliedRange) {#getCellArea-boolean-}
```
public CellArea getCellArea(boolean refreshAppliedRange)
```


يحصل على [CellArea](../../com.aspose.cells/cellarea) حيث ينطبق AutoFilter المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| refreshAppliedRange | boolean | ما إذا كان سيتم تحديث النطاق المطبق. بالنسبة للنطاق المطبق لمرشح تلقائي، قد يتغير الصف الأخير عندما تتغير بيانات الخلايا. إذا كانت هذه العلامة صحيحة، فسيتم إعادة حساب الصف الأخير للنطاق وفقًا لبيانات الخلايا الحالية. |

**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - the area this filter applies to
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFilterColumns() {#getFilterColumns--}
```
public FilterColumnCollection getFilterColumns()
```


يحصل على مجموعة أعمدة الفلترة.

**Returns:**
[FilterColumnCollection](../../com.aspose.cells/filtercolumncollection)
### getRange() {#getRange--}
```
public String getRange()
```


يمثل النطاق الذي ينطبق عليه AutoFilter المحدد.

**Returns:**
java.lang.String
### getShowFilterButton() {#getShowFilterButton--}
```
public boolean getShowFilterButton()
```


يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا.

**Returns:**
boolean
### getSorter() {#getSorter--}
```
public DataSorter getSorter()
```


يحصل على مُرتب البيانات.

**Returns:**
[DataSorter](../../com.aspose.cells/datasorter)
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### matchBlanks(int fieldIndex) {#matchBlanks-int-}
```
public void matchBlanks(int fieldIndex)
```


مطابقة جميع الخلايا الفارغة في القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |

### matchNonBlanks(int fieldIndex) {#matchNonBlanks-int-}
```
public void matchNonBlanks(int fieldIndex)
```


مطابقة جميع الخلايا غير الفارغة في القائمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |

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
public int[] refresh()
```


تحديث الفلاتر التلقائية لإخفاء أو إظهار الصفوف.

**Returns:**
int[] - يرجع جميع فهارس الصفوف المخفية.
### refresh(boolean hideRows) {#refresh-boolean-}
```
public int[] refresh(boolean hideRows)
```


يحصل على مؤشرات جميع الصفوف المخفية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| hideRows | boolean | إذا كان صحيحًا، إخفاء الصفوف المصفاة. |

**Returns:**
int[] - يرجع جميع فهارس الصفوف المخفية.
### removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second) {#removeDateFilter-int-int-int-int-int-int-int-int-}
```
public void removeDateFilter(int fieldIndex, int dateTimeGroupingType, int year, int month, int day, int hour, int minute, int second)
```


يزيل مرشح التاريخ.

**Remarks**

إذا كان DateTimeGroupingType هو Year، فإن المعامل year فقط هو الفعّال. إذا كان DateTiemGroupingType هو Month، فإن المعاملين year و month فقط هما الفعّالان.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| dateTimeGroupingType | int | [DateTimeGroupingType](../../com.aspose.cells/datetimegroupingtype). نوع التجميع |
| سنة | int | السنة. |
| شهر | int | الشهر. |
| يوم | int | اليوم. |
| ساعة | int | الساعة. |
| دقيقة | int | الدقيقة. |
| ثانية | int | الثانية. |

### removeFilter(int fieldIndex) {#removeFilter-int-}
```
public void removeFilter(int fieldIndex)
```


يزيل المرشح المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | فهرس الفلتر المحدد |

### removeFilter(int fieldIndex, String criteria) {#removeFilter-int-java.lang.String-}
```
public void removeFilter(int fieldIndex, String criteria)
```


يزيل مرشحًا لعمود الفلترة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int | الإزاحة الصحيحة للحقول التي تريد أن تستند إليها الفلتر (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| معايير | java.lang.String | المعيار المحدد (سلسلة؛ على سبيل المثال، \"101\"). يمكن أن يكون إما فارغًا أو أحد قيم الخلايا في هذا العمود. |

### setRange(int row, int startColumn, int endColumn) {#setRange-int-int-int-}
```
public void setRange(int row, int startColumn, int endColumn)
```


يضبط النطاق الذي ينطبق عليه AutoFilter المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| startColumn | int | فهرس العمود الابتدائي. |
| endColumn | int | فهرس العمود النهائي. |

### setRange(String value) {#setRange-java.lang.String-}
```
public void setRange(String value)
```


يمثل النطاق الذي ينطبق عليه AutoFilter المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setShowFilterButton(boolean value) {#setShowFilterButton-boolean-}
```
public void setShowFilterButton(boolean value)
```


يشير إلى ما إذا كان زر AutoFilter لهذا العمود مرئيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### showAll() {#showAll--}
```
public void showAll()
```


إظهار جميع الصفوف.

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

