---
title: "GridWorksheet"
second_title: "Aspose.Cells for Java API Reference"
description: "يغلف الكائن الذي يمثل ورقة عمل واحدة."
type: docs
url: /ar/java/com.aspose.gridweb/gridworksheet/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control)
```
public class GridWorksheet extends Control
```

يغلف الكائن الذي يمثل ورقة عمل واحدة.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addAutoFilter(int row, int startColumn, int endColumn)](#addAutoFilter-int-int-int-) | يضبط النطاق الذي ينطبق عليه AutoFilter المحدد. |
| [addCustomFilter(int row, String critira)](#addCustomFilter-int-java.lang.String-) | أضف مرشحًا مخصصًا للصف المحدد. |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | يضبط عرض العمود تلقائيًا. |
| [autoFitColumn(int columnIndex, int firstRow, int lastRow)](#autoFitColumn-int-int-int-) | يضبط عرض العمود تلقائيًا. |
| [autoFitColumns()](#autoFitColumns--) |  |
| [autoFitRow(int rowIndex)](#autoFitRow-int-) | يضبط ارتفاع الصف تلقائيًا. |
| [autoFitRow(int rowIndex, int firstColumn, int lastColumn)](#autoFitRow-int-int-int-) | يضبط ارتفاع الصف تلقائيًا. |
| [autoFitRow(int startRow, int endRow, int startColumn, int endColumn)](#autoFitRow-int-int-int-int-) | يضبط ارتفاع الصف في نطاق مستطيل تلقائيًا. |
| [autoFitRows()](#autoFitRows--) | يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا. |
| [autoFitRows(boolean onlyAuto)](#autoFitRows-boolean-) | يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا. |
| [autoFitRows(int startRow, int endRow)](#autoFitRows-int-int-) | يضبط ارتفاع الصف في نطاق تلقائيًا. |
| [calculateFormula(String formula)](#calculateFormula-java.lang.String-) | يحسب صيغة. |
| [clearComments()](#clearComments--) | يمسح جميع التعليقات في جدول البيانات المصمم. |
| [copy(GridWorksheet sourceSheet)](#copy-com.aspose.gridweb.GridWorksheet-) | ينسخ المحتويات والتنسيقات من ورقة عمل أخرى. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)](#createSubtotal-int-int-int-int-int---) | ينشئ مجموعًا فرعيًا في الورقة. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | ينشئ مجموعًا فرعيًا في الورقة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [filterString(int column, String criteria)](#filterString-int-java.lang.String-) | يضبط الفلتر للعمود. لاحظ أننا سنستدعي AddAutoFilter قبل استدعاء filterString. سلسلة معايير الفلتر. لاحظ أننا نستخدم الفاصلة -> \",\" كحرف تقسيم، لذا يجب ألا يحتوي قيمة الخلية التي تريد تصفيتها على الفاصلة. filterString(10,\"123,456\") يعني أن العمود 10 يجب أن يحتوي على 123 أو 456، filterString(10,\"123\") يعني أن العمود 10 يجب أن يحتوي على 123. قيمة فهرس العمود مفصولة بفواصل، مثال: 123,456,789 أو abc. |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | يثبت الألواح عند الخلية المحددة في ورقة العمل. |
| [freezePanes(String cellName, int freezedRows, int freezedColumns)](#freezePanes-java.lang.String-int-int-) | يثبت الألواح عند الخلية المحددة في ورقة العمل. |
| [getActiveCell()](#getActiveCell--) | يحصل على الخلية النشطة في ورقة العمل. |
| [getBackgroundImage()](#getBackgroundImage--) | يحصل على صورة خلفية ورقة العمل. |
| [getCells()](#getCells--) | يحصل على مجموعة [GridCell](../../com.aspose.gridweb/gridcell). |
| [getClass()](#getClass--) |  |
| [getCodeName()](#getCodeName--) | يمثل اسم رمز ورقة العمل. |
| [getColumnCaption(int column)](#getColumnCaption-int-) | يحصل على تسمية العمود. |
| [getColumnHeaderToolTip(int colIndex)](#getColumnHeaderToolTip-int-) | يحصل على نص تلميح رأس العمود. |
| [getColumnReadonly(int columnIndex)](#getColumnReadonly-int-) | يحصل على ما إذا كان العمود للقراءة فقط. |
| [getComments()](#getComments--) | يحصل على مجموعة [GridComment](../../com.aspose.gridweb/gridcomment). |
| [getDisplayRightToLeft()](#getDisplayRightToLeft--) | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. |
| [getDisplayZeros()](#getDisplayZeros--) | صحيح إذا تم عرض القيم الصفرية. |
| [getFirstVisibleColumn()](#getFirstVisibleColumn--) | يمثل فهرس العمود الأول الظاهر. |
| [getFirstVisibleRow()](#getFirstVisibleRow--) | يمثل فهرس الصف الأول الظاهر. |
| [getFreezedPanes()](#getFreezedPanes--) | يحصل على تجميد الألواح. |
| [getGridActiveCell()](#getGridActiveCell--) | يحصل على الخلية النشطة في ورقة العمل. |
| [getHyperlinks()](#getHyperlinks--) | يحصل على مجموعة [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection). |
| [getIndex()](#getIndex--) | يحصل على فهرس الورقة في مجموعة أوراق العمل. |
| [getIsReadonly(int row, int col)](#getIsReadonly-int-int-) | يحصل على ما إذا كانت الخلية للقراءة فقط. هذا سمة ممتدة لـ GridWeb، ولن تُحفظ في ملف Excel الفعلي. |
| [getName()](#getName--) | يحصل على اسم ورقة العمل. |
| [getOutlineShown()](#getOutlineShown--) | يشير إلى ما إذا كان يُظهر المخطط. |
| [getPictures()](#getPictures--) | يحصل على مجموعة [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--). |
| [getPivotTables()](#getPivotTables--) | يحصل على جداول المحور في ورقة العمل. |
| [getRowCaption(int row)](#getRowCaption-int-) | يحصل على تسمية الصف. |
| [getRowHeaderToolTip(int rowIndex)](#getRowHeaderToolTip-int-) | يحصل على نص تلميح رأس الصف. |
| [getRowReadonly(int rowIndex)](#getRowReadonly-int-) | يحصل على ما إذا كان الصف للقراءة فقط. |
| [getSelected()](#getSelected--) | يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح دفتر العمل. |
| [getShapes()](#getShapes--) | يحصل على مجموعة [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--). |
| [getStandardHeight()](#getStandardHeight--) | يحصل على ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط. |
| [getStandardHeightPixels()](#getStandardHeightPixels--) | يحصل على ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل. |
| [getTabColor()](#getTabColor--) | يمثل لون تبويب ورقة العمل. |
| [getUniqueID()](#getUniqueID--) | يحصل على UniqueID في التحكم |
| [getValidations()](#getValidations--) | يحصل على مجموعة إعدادات التحقق من صحة البيانات في ورقة العمل. |
| [getVisible()](#getVisible--) | يشير إلى ما إذا كان اسم هذه الورقة معروضًا في علامات تبويب الورقة في التحكم. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن [GridWorkbook](../../com.aspose.gridweb/gridworkbook) لمجموعة أوراق العمل. |
| [getZoom()](#getZoom--) | يمثل عامل التحجيم بالنسبة المئوية. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | يقوم بتجميع الصفوف. |
| [hashCode()](#hashCode--) |  |
| [isGridlinesVisible()](#isGridlinesVisible--) | يحصل على قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true. |
| [isProtected()](#isProtected--) | يشير إلى ما إذا كانت ورقة العمل محمية. |
| [isSummaryRowBelow()](#isSummaryRowBelow--) | يشير إلى ما إذا كان سيتم وضع صف الملخص أسفل صفوف التفاصيل في المخطط التفصيلي. |
| [moveTo(int index)](#moveTo-int-) | ينقل الورقة إلى موقع آخر في جدول البيانات. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [refreshFilter()](#refreshFilter--) | تحديث الفلاتر التلقائية لإخفاء أو إظهار الصفوف. |
| [removeAutoFilter()](#removeAutoFilter--) | إزالة الفلتر التلقائي لورقة العمل. |
| [removeSubtotal()](#removeSubtotal--) | يزيل الإجمالي الفرعي الذي تم إنشاؤه بواسطة طريقة CreateSubtotal في الورقة. |
| [resetFilter(int fieldIndex)](#resetFilter-int-) | الإزاحة الصحيحة للحقول التي تريد تطبيقها، بناءً على أول عمود تصفية (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0). |
| [setActiveCell(String value)](#setActiveCell-java.lang.String-) | يضبط الخلية النشطة في ورقة العمل. |
| [setAllCellsEditable()](#setAllCellsEditable--) | يجعل جميع الخلايا قابلة للتحرير. هذا سمة موسعة. |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | يجعل جميع الخلايا للقراءة فقط. هذه سمة موسعة، لاحظ أن هذه السمة لا يمكن الاحتفاظ بها في الخلية الفعلية، إذا كنت تريد الحفاظ على الحماية يرجى استخدام setProtect. |
| [setBackgroundImage(byte[] value)](#setBackgroundImage-byte---) | يضبط صورة خلفية ورقة العمل. |
| [setColumnCaption(int column, String caption)](#setColumnCaption-int-java.lang.String-) | يضبط التسمية للعمود. يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel. |
| [setColumnHeaderToolTip(int colIndex, String toolTip)](#setColumnHeaderToolTip-int-java.lang.String-) | يضبط نص تلميح أداة رأس العمود. |
| [setColumnReadonly(int columnIndex, boolean isReadonly)](#setColumnReadonly-int-boolean-) | يضبط عمودًا للقراءة فقط بحيث لا يستطيع المستخدم حذفه من جانب العميل. |
| [setDisplayRightToLeft(boolean value)](#setDisplayRightToLeft-boolean-) | يشير إلى ما إذا كانت ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. |
| [setDisplayZeros(boolean value)](#setDisplayZeros-boolean-) | صحيح إذا تم عرض القيم الصفرية. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | يجعل نطاقًا من الخلايا قابلاً للتحرير. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells اجعل جميع الخلايا للقراءة فقط عن طريق استدعاء طريقة SetAllCellsReadonly. |
| [setFirstVisibleColumn(int value)](#setFirstVisibleColumn-int-) | يمثل فهرس العمود الأول الظاهر. |
| [setFirstVisibleRow(int value)](#setFirstVisibleRow-int-) | يمثل فهرس الصف الأول الظاهر. |
| [setGridActiveCell(GridCell value)](#setGridActiveCell-com.aspose.gridweb.GridCell-) | يضبط الخلية النشطة في ورقة العمل. |
| [setGridlinesVisible(boolean value)](#setGridlinesVisible-boolean-) | يضبط قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true. |
| [setIsReadonly(int row, int col, boolean value)](#setIsReadonly-int-int-boolean-) | يضبط ما إذا كانت الخلية للقراءة فقط. هذه سمة موسعة لـ GridWeb، ولن تُحفظ في ملف Excel الفعلي. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم ورقة العمل. |
| [setOutlineShown(boolean value)](#setOutlineShown-boolean-) | يشير إلى ما إذا كان يُظهر المخطط. |
| [setProtect()](#setProtect--) | يحمي ورقة العمل. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | يجعل نطاقًا من الخلايا للقراءة فقط. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells أولاً اجعل جميع الخلايا قابلة للتحرير عن طريق استدعاء طريقة SetAllCellsEditable. |
| [setRowCaption(int row, String caption)](#setRowCaption-int-java.lang.String-) | يضبط التسمية للصف. |
| [setRowHeaderToolTip(int rowIndex, String toolTip)](#setRowHeaderToolTip-int-java.lang.String-) | يضبط نص تلميح أداة رأس الصف. |
| [setRowReadonly(int rowIndex, boolean isReadonly)](#setRowReadonly-int-boolean-) | يضبط صفًا للقراءة فقط بحيث لا يستطيع المستخدم حذفه من جانب العميل. |
| [setSelected(boolean value)](#setSelected-boolean-) | يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح دفتر العمل. |
| [setStandardHeight(double value)](#setStandardHeight-double-) | يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط. |
| [setStandardHeightPixels(int value)](#setStandardHeightPixels-int-) | يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل. |
| [setSummaryRowBelow(boolean value)](#setSummaryRowBelow-boolean-) | يشير إلى ما إذا كان سيتم وضع صف الملخص أسفل صفوف التفاصيل في المخطط التفصيلي. |
| [setTabColor(Color value)](#setTabColor-com.aspose.gridweb.Color-) | يمثل لون تبويب ورقة العمل. |
| [setVisible(boolean value)](#setVisible-boolean-) | يشير إلى ما إذا كان اسم هذه الورقة معروضًا في علامات تبويب الورقة في التحكم. |
| [setZoom(int value)](#setZoom-int-) | يمثل عامل التحجيم بالنسبة المئوية. |
| [toString()](#toString--) |  |
| [unFreezePanes()](#unFreezePanes--) | يفك تجميد الألواح في ورقة العمل. |
| [unGroupRows(int firstIndex, int lastIndex)](#unGroupRows-int-int-) | يفك تجميع الصفوف. |
| [unProtect()](#unProtect--) | إلغاء حماية ورقة العمل. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addAutoFilter(int row, int startColumn, int endColumn) {#addAutoFilter-int-int-int-}
```
public void addAutoFilter(int row, int startColumn, int endColumn)
```


يضبط النطاق الذي ينطبق عليه AutoFilter المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| startColumn | int | فهرس العمود الابتدائي. |
| endColumn | int | فهرس العمود النهائي. |

### addCustomFilter(int row, String critira) {#addCustomFilter-int-java.lang.String-}
```
public void addCustomFilter(int row, String critira)
```


أضف مرشحًا مخصصًا للصف المحدد.

**Remarks**

سلسلة معايير الفلتر. لاحظ أننا نستخدم , و ; كحرف تقسيم، لذا يجب ألا يحتوي قيمة الخلية على تلك الأحرف. أدناه أمثلة على سلاسل المعايير //column 0 with value 12.3 CELL0 = 12.3 //column 1 with value ABC CELL1 = ABC //column 0 with value 123 or 456 or ABC and column 1 with value ABC CELL0 = 123,456,ABC; CELL1 = ABC

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int |  |
| معايير | java.lang.String |  |

### autoFitColumn(int columnIndex) {#autoFitColumn-int-}
```
public void autoFitColumn(int columnIndex)
```


يضبط عرض العمود تلقائيًا.

**Remarks**

AutoFitColumn هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |

### autoFitColumn(int columnIndex, int firstRow, int lastRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int firstRow, int lastRow)
```


يضبط عرض العمود تلقائيًا.

**Remarks**

تقوم هذه الطريقة بضبط عرض الصف تلقائيًا بناءً على المحتوى في نطاق الخلايا داخل الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| firstRow | int | فهرس الصف الأول. |
| lastRow | int | فهرس الصف الأخير. |

### autoFitColumns() {#autoFitColumns--}
```
public void autoFitColumns()
```




### autoFitRow(int rowIndex) {#autoFitRow-int-}
```
public void autoFitRow(int rowIndex)
```


يضبط ارتفاع الصف تلقائيًا.

**Remarks**

AutoFitRow هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |

### autoFitRow(int rowIndex, int firstColumn, int lastColumn) {#autoFitRow-int-int-int-}
```
public void autoFitRow(int rowIndex, int firstColumn, int lastColumn)
```


يضبط ارتفاع الصف تلقائيًا.

**Remarks**

تقوم هذه الطريقة بضبط عرض الصف تلقائيًا بناءً على المحتوى في نطاق الخلايا داخل الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| firstColumn | int | فهرس العمود الأول. |
| lastColumn | int | فهرس العمود الأخير. |

### autoFitRow(int startRow, int endRow, int startColumn, int endColumn) {#autoFitRow-int-int-int-int-}
```
public void autoFitRow(int startRow, int endRow, int startColumn, int endColumn)
```


يضبط ارتفاع الصف في نطاق مستطيل تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| endRow | int | فهرس الصف النهائي. |
| startColumn | int | فهرس العمود الابتدائي. |
| endColumn | int | فهرس العمود النهائي. |

### autoFitRows() {#autoFitRows--}
```
public void autoFitRows()
```


يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا.

### autoFitRows(boolean onlyAuto) {#autoFitRows-boolean-}
```
public void autoFitRows(boolean onlyAuto)
```


يضبط جميع الصفوف في ورقة العمل هذه تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| onlyAuto | boolean | صحيح، يقوم بتعديل ارتفاع الصف تلقائيًا فقط عندما لا يكون ارتفاع الصف مخصصًا. |

### autoFitRows(int startRow, int endRow) {#autoFitRows-int-int-}
```
public void autoFitRows(int startRow, int endRow)
```


يضبط ارتفاع الصف في نطاق تلقائيًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | فهرس الصف الابتدائي. |
| endRow | int | فهرس الصف النهائي. |

### calculateFormula(String formula) {#calculateFormula-java.lang.String-}
```
public Object calculateFormula(String formula)
```


يحسب صيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String |  |

**Returns:**
java.lang.Object - 
### clearComments() {#clearComments--}
```
public void clearComments()
```


يمسح جميع التعليقات في جدول البيانات المصمم.

### copy(GridWorksheet sourceSheet) {#copy-com.aspose.gridweb.GridWorksheet-}
```
public void copy(GridWorksheet sourceSheet)
```


ينسخ المحتويات والتنسيقات من ورقة عمل أخرى.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sourceSheet | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) | ورقة العمل المصدر. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList) {#createSubtotal-int-int-int-int-int---}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList)
```


ينشئ مجموعًا فرعيًا في الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnNameRowIndex | int | فهرس الصف لصف اسم العمود. |
| dataRows | int | عدد صفوف البيانات. |
| groupByColumnIndex | int | فهرس العمود للعمود الذي سيتم تجميعه. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). نوع دالة المجموع الفرعي. |
| subtotalColumnIndexList | int[] | فهارس الأعمدة التي سيتم جمعها فرعيًا. |

### createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString) {#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-}
```
public void createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)
```


ينشئ مجموعًا فرعيًا في الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnNameRowIndex | int | فهرس الصف لصف اسم العمود. |
| dataRows | int | عدد صفوف البيانات. |
| groupByColumnIndex | int | فهرس العمود للعمود الذي سيتم تجميعه. |
| subtotalFunction | int | [SubtotalFunction](../../com.aspose.gridweb/subtotalfunction). نوع دالة المجموع الفرعي. |
| subtotalColumnIndexList | int[] | فهارس الأعمدة التي سيتم جمعها فرعيًا. |
| functionLabel | java.lang.String | تسمية دالة المجموع الفرعي. |
| grandCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | نمط سطر الإجمالي الكلي. |
| subtotalCellStyle | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | نمط سطر المجموع الفرعي. |
| numberType | int | [NumberType](../../com.aspose.gridweb/numbertype). نوع الرقم لخلايا نتيجة المجموع الفرعي. |
| customString | java.lang.String | سلسلة تنسيق مخصصة لخلايا نتيجة المجموع الفرعي. يمكن أن تكون فارغة. |

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
### filterString(int column, String criteria) {#filterString-int-java.lang.String-}
```
public void filterString(int column, String criteria)
```


يضبط الفلتر للعمود. لاحظ أننا سنستدعي AddAutoFilter قبل استدعاء filterString. سلسلة معايير الفلتر. لاحظ أننا نستخدم الفاصلة -> \",\" كحرف تقسيم، لذا يجب ألا يحتوي قيمة الخلية التي تريد تصفيتها على الفاصلة. filterString(10,\"123,456\") يعني أن العمود 10 يجب أن يحتوي على 123 أو 456، filterString(10,\"123\") يعني أن العمود 10 يجب أن يحتوي على 123. قيمة فهرس العمود مفصولة بفواصل، مثال: 123,456,789 أو abc.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int |  |
| معايير | java.lang.String |  |

### freezePanes(int row, int column, int freezedRows, int freezedColumns) {#freezePanes-int-int-int-int-}
```
public void freezePanes(int row, int column, int freezedRows, int freezedColumns)
```


يثبت الألواح عند الخلية المحددة في ورقة العمل.

**Remarks**

لا يمكن أن يكون كل من فهرس الصف وفهرس العمود صفرًا. كما لا يمكن أن يكون عدد الصفوف وعدد الأعمدة صفرًا.

المعاملان الأولان يحددان موضع التجميد والمعاملان الأخيران يحددان المنطقة المجمدة في الجزء العلوي الأيسر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| عمود | int | فهرس العمود. |
| freezedRows | int | عدد الصفوف المرئية في الجزء العلوي، لا يزيد عن فهرس الصف. |
| freezedColumns | int | عدد الأعمدة المرئية في الجزء الأيسر، لا يزيد عن فهرس العمود. |

### freezePanes(String cellName, int freezedRows, int freezedColumns) {#freezePanes-java.lang.String-int-int-}
```
public void freezePanes(String cellName, int freezedRows, int freezedColumns)
```


يثبت الألواح عند الخلية المحددة في ورقة العمل.

**Remarks**

لا يمكن أن يكون كل من فهرس الصف وفهرس العمود صفرًا. كما لا يمكن أن يكون عدد الصفوف وعدد الأعمدة صفرًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellName | java.lang.String | اسم الخلية. |
| freezedRows | int | عدد الصفوف المرئية في الجزء العلوي، لا يزيد عن فهرس الصف. |
| freezedColumns | int | عدد الأعمدة المرئية في الجزء الأيسر، لا يزيد عن فهرس العمود. |

### getActiveCell() {#getActiveCell--}
```
public String getActiveCell()
```


يحصل على الخلية النشطة في ورقة العمل.

**Returns:**
java.lang.String
### getBackgroundImage() {#getBackgroundImage--}
```
public byte[] getBackgroundImage()
```


يحصل على صورة خلفية ورقة العمل.

**Returns:**
byte[]
### getCells() {#getCells--}
```
public GridCells getCells()
```


يحصل على مجموعة [GridCell](../../com.aspose.gridweb/gridcell).

**Returns:**
[GridCells](../../com.aspose.gridweb/gridcells)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCodeName() {#getCodeName--}
```
public String getCodeName()
```


يمثل اسم رمز ورقة العمل.

**Remarks**

لا يمكنك تغيير اسم الكود بينما يحتوي ملف القالب على VBA/ماكرو.

**Returns:**
java.lang.String
### getColumnCaption(int column) {#getColumnCaption-int-}
```
public String getColumnCaption(int column)
```


يحصل على تسمية العمود. إذا لم يتم تعيين التسمية، يرجع سلسلة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |

**Returns:**
java.lang.String - تسمية العمود. إذا لم يتم تعيين التسمية، يرجع سلسلة فارغة.
### getColumnHeaderToolTip(int colIndex) {#getColumnHeaderToolTip-int-}
```
public String getColumnHeaderToolTip(int colIndex)
```


يحصل على نص تلميح رأس العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| colIndex | int | فهرس العمود. |

**Returns:**
java.lang.String - نص التلميح.
### getColumnReadonly(int columnIndex) {#getColumnReadonly-int-}
```
public boolean getColumnReadonly(int columnIndex)
```


يتحقق مما إذا كان العمود للقراءة فقط. هذه طريقة موسعة من GridWeb تحديدًا، ولن تُحفظ أو تُؤثر في ملف Excel الفعلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |

**Returns:**
boolean - إذا كان للقراءة فقط يرجع true.
### getComments() {#getComments--}
```
public GridCommentCollection getComments()
```


يحصل على مجموعة [GridComment](../../com.aspose.gridweb/gridcomment).

**Returns:**
[GridCommentCollection](../../com.aspose.gridweb/gridcommentcollection)
### getDisplayRightToLeft() {#getDisplayRightToLeft--}
```
public boolean getDisplayRightToLeft()
```


يشير إلى ما إذا كان ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false.

**Returns:**
boolean
### getDisplayZeros() {#getDisplayZeros--}
```
public boolean getDisplayZeros()
```


صحيح إذا تم عرض القيم الصفرية.

**Returns:**
boolean
### getFirstVisibleColumn() {#getFirstVisibleColumn--}
```
public int getFirstVisibleColumn()
```


يمثل فهرس العمود الأول الظاهر.

**Returns:**
int
### getFirstVisibleRow() {#getFirstVisibleRow--}
```
public int getFirstVisibleRow()
```


يمثل فهرس الصف الأول الظاهر.

**Returns:**
int
### getFreezedPanes() {#getFreezedPanes--}
```
public int[] getFreezedPanes()
```


يحصل على تجميد الألواح.

**Returns:**
int[] - إرجاع null يعني أن ورقة العمل غير مُجمدة 0:فهرس الصف;1:العمود;2:الصفوف المجمدة;3:الصفوف المجمدة
### getGridActiveCell() {#getGridActiveCell--}
```
public GridCell getGridActiveCell()
```


يحصل على الخلية النشطة في ورقة العمل.

**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getHyperlinks() {#getHyperlinks--}
```
public GridHyperlinkCollection getHyperlinks()
```


يحصل على مجموعة [GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection).

**Returns:**
[GridHyperlinkCollection](../../com.aspose.gridweb/gridhyperlinkcollection)
### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على فهرس الورقة في مجموعة أوراق العمل.

**Returns:**
int
### getIsReadonly(int row, int col) {#getIsReadonly-int-int-}
```
public boolean getIsReadonly(int row, int col)
```


يحصل على ما إذا كانت الخلية للقراءة فقط. هذا سمة ممتدة لـ GridWeb، ولن تُحفظ في ملف Excel الفعلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int |  |
| col | int |  |

**Returns:**
boolean
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم ورقة العمل.

**Remarks**

الحد الأقصى لطول اسم الورقة هو 31. ولا يمكنك تعيين نفس الاسم (بدون حساسية لحالة الأحرف) لورقتين عمل. على سبيل المثال، لا يمكنك تعيين "SheetName1" للورقة الأولى وتعيين "SHEETNAME1" للورقة الثانية.

**Returns:**
java.lang.String
### getOutlineShown() {#getOutlineShown--}
```
public boolean getOutlineShown()
```


يشير إلى ما إذا كان يُظهر المخطط.

**Returns:**
boolean
### getPictures() {#getPictures--}
```
public GridPictureCollection getPictures()
```


يحصل على مجموعة [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--).

**Returns:**
[GridPictureCollection](../../com.aspose.gridweb/gridpicturecollection)
### getPivotTables() {#getPivotTables--}
```
public GridPivotTableCollection getPivotTables()
```


يحصل على جداول المحور في ورقة العمل.

**Returns:**
[GridPivotTableCollection](../../com.aspose.gridweb/gridpivottablecollection)
### getRowCaption(int row) {#getRowCaption-int-}
```
public String getRowCaption(int row)
```


يحصل على تسمية الصف. إذا لم يتم تعيين التسمية، يرجع سلسلة فارغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |

**Returns:**
java.lang.String - تسمية الصف. إذا لم يتم تعيين التسمية، يرجع سلسلة فارغة.
### getRowHeaderToolTip(int rowIndex) {#getRowHeaderToolTip-int-}
```
public String getRowHeaderToolTip(int rowIndex)
```


يحصل على نص تلميح رأس الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |

**Returns:**
java.lang.String - نص التلميح.
### getRowReadonly(int rowIndex) {#getRowReadonly-int-}
```
public boolean getRowReadonly(int rowIndex)
```


يحصل إذا كان الصف للقراءة فقط. هذه طريقة موسعة لـ GridWeb تحديدًا، لن تُحفظ وتؤثر في ملف Excel الفعلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |

**Returns:**
boolean - إذا كان للقراءة فقط يرجع true.
### getSelected() {#getSelected--}
```
public boolean getSelected()
```


يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح دفتر العمل.

**Returns:**
boolean
### getShapes() {#getShapes--}
```
public GridShapeCollection getShapes()
```


يحصل على مجموعة [getPictures()](../../com.aspose.gridweb/gridworksheet\\#getPictures--).

**Returns:**
[GridShapeCollection](../../com.aspose.gridweb/gridshapecollection)
### getStandardHeight() {#getStandardHeight--}
```
public double getStandardHeight()
```


يحصل على ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط.

**Returns:**
double
### getStandardHeightPixels() {#getStandardHeightPixels--}
```
public int getStandardHeightPixels()
```


يحصل على ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل.

**Returns:**
int
### getTabColor() {#getTabColor--}
```
public Color getTabColor()
```


يمثل لون تبويب ورقة العمل.

**Remarks**

هذه الميزة مدعومة فقط في ExcelXP (Excel2002) والإصدارات الأحدث. إذا حفظت الملف بصيغة Excel97 أو Excel2000، سيتم حذفها.

**Returns:**
[Color](../../com.aspose.gridweb/color)
### getUniqueID() {#getUniqueID--}
```
public String getUniqueID()
```


يحصل على UniqueID في التحكم

**Returns:**
java.lang.String
### getValidations() {#getValidations--}
```
public GridValidationCollection getValidations()
```


يحصل على مجموعة إعدادات التحقق من صحة البيانات في ورقة العمل.

**Returns:**
[GridValidationCollection](../../com.aspose.gridweb/gridvalidationcollection)
### getVisible() {#getVisible--}
```
public boolean getVisible()
```


يشير إلى ما إذا كان اسم هذه الورقة معروضًا في علامات تبويب الورقة في التحكم.

**Returns:**
boolean
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```


يحصل على كائن [GridWorkbook](../../com.aspose.gridweb/gridworkbook) لمجموعة أوراق العمل.

**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getZoom() {#getZoom--}
```
public int getZoom()
```


يمثل معامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400.

**Returns:**
int
### groupRows(int firstIndex, int lastIndex, boolean isHidden) {#groupRows-int-int-boolean-}
```
public void groupRows(int firstIndex, int lastIndex, boolean isHidden)
```


يقوم بتجميع الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول لتجميعه. |
| lastIndex | int | فهرس الصف الأخير لتجميعه. |
| isHidden | boolean | يحدد ما إذا كانت الصفوف المجمعة مخفية. |

### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isGridlinesVisible() {#isGridlinesVisible--}
```
public boolean isGridlinesVisible()
```


يحصل على قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true.

**Returns:**
boolean
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


يشير إلى ما إذا كانت ورقة العمل محمية.

**Returns:**
boolean
### isSummaryRowBelow() {#isSummaryRowBelow--}
```
public boolean isSummaryRowBelow()
```


يشير إلى ما إذا كان سيتم وضع صف الملخص أسفل صفوف التفاصيل في المخطط التفصيلي.

**Returns:**
boolean
### moveTo(int index) {#moveTo-int-}
```
public void moveTo(int index)
```


ينقل الورقة إلى موقع آخر في جدول البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس الورقة الوجهة. |

### notify() {#notify--}
```
public final native void notify()
```




### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```




### refreshFilter() {#refreshFilter--}
```
public void refreshFilter()
```


تحديث الفلاتر التلقائية لإخفاء أو إظهار الصفوف.

### removeAutoFilter() {#removeAutoFilter--}
```
public void removeAutoFilter()
```


إزالة الفلتر التلقائي لورقة العمل.

### removeSubtotal() {#removeSubtotal--}
```
public void removeSubtotal()
```


يزيل الإجمالي الفرعي الذي تم إنشاؤه بواسطة طريقة CreateSubtotal في الورقة.

### resetFilter(int fieldIndex) {#resetFilter-int-}
```
public void resetFilter(int fieldIndex)
```


الإزاحة الصحيحة للحقول التي تريد تطبيقها، بناءً على أول عمود تصفية (من اليسار في القائمة؛ الحقل الأيسر هو الحقل 0).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| fieldIndex | int |  |

### setActiveCell(String value) {#setActiveCell-java.lang.String-}
```
public void setActiveCell(String value)
```


يضبط الخلية النشطة في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setAllCellsEditable() {#setAllCellsEditable--}
```
public void setAllCellsEditable()
```


يجعل جميع الخلايا قابلة للتحرير. هذا سمة موسعة.

### setAllCellsReadonly() {#setAllCellsReadonly--}
```
public void setAllCellsReadonly()
```


يجعل جميع الخلايا للقراءة فقط. هذه سمة موسعة، لاحظ أن هذه السمة لا يمكن الاحتفاظ بها في الخلية الفعلية، إذا كنت تريد الحفاظ على الحماية يرجى استخدام setProtect.

### setBackgroundImage(byte[] value) {#setBackgroundImage-byte---}
```
public void setBackgroundImage(byte[] value)
```


يضبط صورة خلفية ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | byte[] |  |

### setColumnCaption(int column, String caption) {#setColumnCaption-int-java.lang.String-}
```
public void setColumnCaption(int column, String caption)
```


يضبط التسمية للعمود. يرجى ملاحظة أن هذه سمة امتداد ولا يمكن الاحتفاظ بها في ملف Excel.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| عمود | int | فهرس العمود. |
| التسمية | java.lang.String | تسمية العمود. مرّر null أو سلسلة فارغة إذا أردت إلغاء التسمية. |

### setColumnHeaderToolTip(int colIndex, String toolTip) {#setColumnHeaderToolTip-int-java.lang.String-}
```
public void setColumnHeaderToolTip(int colIndex, String toolTip)
```


يضبط نص تلميح أداة رأس العمود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| colIndex | int | فهرس العمود. |
| تلميح الأدوات | java.lang.String | نص تلميح الأدوات. |

### setColumnReadonly(int columnIndex, boolean isReadonly) {#setColumnReadonly-int-boolean-}
```
public void setColumnReadonly(int columnIndex, boolean isReadonly)
```


يضبط العمود للقراءة فقط بحيث لا يستطيع المستخدم حذفه من جانب العميل. هذه طريقة موسعة لـ GridWeb تحديدًا، لن تُحفظ وتؤثر في ملف Excel الفعلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود. |
| isReadonly | boolean | صحيح أو خطأ. |

### setDisplayRightToLeft(boolean value) {#setDisplayRightToLeft-boolean-}
```
public void setDisplayRightToLeft(boolean value)
```


يشير إلى ما إذا كان ورقة العمل المحددة تُعرض من اليمين إلى اليسار بدلاً من اليسار إلى اليمين. القيمة الافتراضية هي false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setDisplayZeros(boolean value) {#setDisplayZeros-boolean-}
```
public void setDisplayZeros(boolean value)
```


صحيح إذا تم عرض القيم الصفرية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setEditableRange(int startRow, int startColumn, int rows, int columns) {#setEditableRange-int-int-int-int-}
```
public void setEditableRange(int startRow, int startColumn, int rows, int columns)
```


يجعل نطاقًا من الخلايا قابلًا للتحرير. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells اجعل جميع الخلايا للقراءة فقط باستدعاء طريقة SetAllCellsReadonly. ثم استدعِ هذه الطريقة لتحديد نطاق الخلايا الذي يجب أن يكون قابلًا للتحرير.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية للنطاق. |
| startColumn | int | عمود البداية للنطاق. |
| الصفوف | int | عدد الصفوف. |
| الأعمدة | int | عدد الأعمدة. |

### setFirstVisibleColumn(int value) {#setFirstVisibleColumn-int-}
```
public void setFirstVisibleColumn(int value)
```


يمثل فهرس العمود الأول الظاهر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setFirstVisibleRow(int value) {#setFirstVisibleRow-int-}
```
public void setFirstVisibleRow(int value)
```


يمثل فهرس الصف الأول الظاهر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setGridActiveCell(GridCell value) {#setGridActiveCell-com.aspose.gridweb.GridCell-}
```
public void setGridActiveCell(GridCell value)
```


يضبط الخلية النشطة في ورقة العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridCell](../../com.aspose.gridweb/gridcell) |  |

### setGridlinesVisible(boolean value) {#setGridlinesVisible-boolean-}
```
public void setGridlinesVisible(boolean value)
```


يضبط قيمة تشير إلى ما إذا كانت خطوط الشبكة مرئية. القيمة الافتراضية هي true.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setIsReadonly(int row, int col, boolean value) {#setIsReadonly-int-int-boolean-}
```
public void setIsReadonly(int row, int col, boolean value)
```


يضبط ما إذا كانت الخلية للقراءة فقط. هذه سمة موسعة لـ GridWeb، ولن تُحفظ في ملف Excel الفعلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int |  |
| col | int |  |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم ورقة العمل.

**Remarks**

الحد الأقصى لطول اسم الورقة هو 31. ولا يمكنك تعيين نفس الاسم (بدون حساسية لحالة الأحرف) لورقتين عمل. على سبيل المثال، لا يمكنك تعيين "SheetName1" للورقة الأولى وتعيين "SHEETNAME1" للورقة الثانية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOutlineShown(boolean value) {#setOutlineShown-boolean-}
```
public void setOutlineShown(boolean value)
```


يشير إلى ما إذا كان يُظهر المخطط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setProtect() {#setProtect--}
```
public void setProtect()
```


يحمي ورقة العمل.

**Remarks**

تحمي هذه الطريقة ورقة العمل بدون كلمة مرور. يمكنها حماية ورقة العمل في جميع إصدارات ملف Excel.

### setReadonlyRange(int startRow, int startColumn, int rows, int columns) {#setReadonlyRange-int-int-int-int-}
```
public void setReadonlyRange(int startRow, int startColumn, int rows, int columns)
```


يجعل نطاقًا من الخلايا للقراءة فقط. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells أولاً اجعل جميع الخلايا قابلة للتحرير باستدعاء طريقة SetAllCellsEditable. ثم استدعِ هذه الطريقة لتحديد نطاق الخلايا الذي يجب أن يكون للقراءة فقط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| startRow | int | صف البداية للنطاق. |
| startColumn | int | عمود البداية للنطاق. |
| الصفوف | int | عدد الصفوف. |
| الأعمدة | int | عدد الأعمدة. |

### setRowCaption(int row, String caption) {#setRowCaption-int-java.lang.String-}
```
public void setRowCaption(int row, String caption)
```


يضبط التسمية للصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | فهرس الصف. |
| التسمية | java.lang.String | تسمية الصف. مرّر null أو سلسلة فارغة إذا أردت إلغاء التسمية. |

### setRowHeaderToolTip(int rowIndex, String toolTip) {#setRowHeaderToolTip-int-java.lang.String-}
```
public void setRowHeaderToolTip(int rowIndex, String toolTip)
```


يضبط نص تلميح أداة رأس الصف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| تلميح الأدوات | java.lang.String | نص تلميح الأدوات. |

### setRowReadonly(int rowIndex, boolean isReadonly) {#setRowReadonly-int-boolean-}
```
public void setRowReadonly(int rowIndex, boolean isReadonly)
```


يضبط الصف للقراءة فقط بحيث لا يستطيع المستخدم حذفه من جانب العميل. هذه طريقة موسعة لـ GridWeb تحديدًا، لن تُحفظ وتؤثر في ملف Excel الفعلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowIndex | int | فهرس الصف. |
| isReadonly | boolean | صحيح أو خطأ. |

### setSelected(boolean value) {#setSelected-boolean-}
```
public void setSelected(boolean value)
```


يشير إلى ما إذا كانت ورقة العمل هذه مختارة عند فتح دفتر العمل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStandardHeight(double value) {#setStandardHeight-double-}
```
public void setStandardHeight(double value)
```


يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة النقاط.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | double |  |

### setStandardHeightPixels(int value) {#setStandardHeightPixels-int-}
```
public void setStandardHeightPixels(int value)
```


يضبط ارتفاع الصف الافتراضي في هذه الورقة، بوحدة البكسل.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setSummaryRowBelow(boolean value) {#setSummaryRowBelow-boolean-}
```
public void setSummaryRowBelow(boolean value)
```


يشير إلى ما إذا كان سيتم وضع صف الملخص أسفل صفوف التفاصيل في المخطط التفصيلي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setTabColor(Color value) {#setTabColor-com.aspose.gridweb.Color-}
```
public void setTabColor(Color value)
```


يمثل لون تبويب ورقة العمل.

**Remarks**

هذه الميزة مدعومة فقط في ExcelXP (Excel2002) والإصدارات الأحدث. إذا حفظت الملف بصيغة Excel97 أو Excel2000، سيتم حذفها.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Color](../../com.aspose.gridweb/color) |  |

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يشير إلى ما إذا كان اسم هذه الورقة معروضًا في علامات تبويب الورقة في التحكم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setZoom(int value) {#setZoom-int-}
```
public void setZoom(int value)
```


يمثل معامل التحجيم بالنسبة المئوية. يجب أن يكون بين 10 و 400.

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
### unFreezePanes() {#unFreezePanes--}
```
public void unFreezePanes()
```


يفك تجميد الألواح في ورقة العمل.

### unGroupRows(int firstIndex, int lastIndex) {#unGroupRows-int-int-}
```
public void unGroupRows(int firstIndex, int lastIndex)
```


يفك تجميع الصفوف.

**Remarks**

يزيل فقط معلومات المجموعة الخارجية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول الذي سيتم فك تجميعه. |
| lastIndex | int | فهرس الصف الأخير الذي سيتم فك تجميعه. |

### unProtect() {#unProtect--}
```
public void unProtect()
```


إلغاء حماية ورقة العمل.

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

