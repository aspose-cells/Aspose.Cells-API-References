---
title: "تصميم ورقة العمل"
second_title: "Aspose.Cells for Java API Reference"
description: "موروث من WebWorksheet."
type: docs
url: /ar/java/com.aspose.gridweb/worksheetdesign/
---

**Inheritance:**
java.lang.Object, [com.aspose.gridweb.Control](../../com.aspose.gridweb/control), [com.aspose.gridweb.WebWorksheet](../../com.aspose.gridweb/webworksheet)
```
public class WorksheetDesign extends WebWorksheet
```

موروث من WebWorksheet. يُستخدم في وقت التصميم فقط.
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [WorksheetDesign()](#WorksheetDesign--) | المنشئ الافتراضي. |
| [WorksheetDesign(MainWeb mw, GridWorksheet gwk)](#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-) | البناء مع MainWeb و GridWorksheet |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [autoFitColumn(int columnIndex)](#autoFitColumn-int-) | يضبط عرض العمود تلقائيًا. |
| [autoFitColumn(int columnIndex, int startRow, int endRow)](#autoFitColumn-int-int-int-) | يضبط عرض العمود تلقائيًا. |
| [cancelNewBindRow()](#cancelNewBindRow--) | يلغي ويحذف الصف المرتبط المضاف حديثًا. |
| [commitNewBindRow()](#commitNewBindRow--) | يؤكد الصف المرتبط المضاف حديثًا ويضيفه إلى مصدر البيانات. |
| [copy(WebWorksheet source)](#copy-com.aspose.gridweb.WebWorksheet-) | ينسخ من كائن ورقة عمل آخر. |
| [createAutoGenratedColumns()](#createAutoGenratedColumns--) | بعد تعيين مصدر بيانات للورقة، استدعِ هذه الطريقة لتوليد الأعمدة المرتبطة تلقائيًا. |
| [createNewBindRow()](#createNewBindRow--) | ينشئ صفًا مرتبطًا جديدًا ويربطه بمصدر البيانات. |
| [createSubtotal(int columnNameRowIndex, int dataRows, int groupByColumnIndex, int subtotalFunction, int[] subtotalColumnIndexList, String functionLabel, GridTableItemStyle grandCellStyle, GridTableItemStyle subtotalCellStyle, int numberType, String customString)](#createSubtotal-int-int-int-int-int---java.lang.String-com.aspose.gridweb.GridTableItemStyle-com.aspose.gridweb.GridTableItemStyle-int-java.lang.String-) | ينشئ مجموعًا فرعيًا في الورقة. |
| [dataBind()](#dataBind--) | اربط الورقة بمصدر البيانات. |
| [deleteBindRow(int rowNum)](#deleteBindRow-int-) | يحذف صفًا مرتبطًا. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [freezePanes(int row, int column, int freezedRows, int freezedColumns)](#freezePanes-int-int-int-int-) | يثبت الألواح عند الخلية المحددة في ورقة العمل. |
| [getBindStartColumn()](#getBindStartColumn--) | في وضع ربط البيانات، يشير BindStartRow و BindStartColumn إلى موضع الشبكة للربط بمصدر البيانات. |
| [getBindStartRow()](#getBindStartRow--) | في وضع ربط البيانات، يشير BindStartRow و BindStartColumn إلى موضع الشبكة للربط بمصدر البيانات. |
| [getBindingSource()](#getBindingSource--) | كائن مصدر البيانات المرتبط فعليًا أثناء التشغيل. |
| [getClass()](#getClass--) |  |
| [getCurrentBindRows()](#getCurrentBindRows--) | يحصل على عدد الصفوف المرتبطة في وضع ربط البيانات. |
| [getDataMember()](#getDataMember--) | يحصل على DataMember من مصدر البيانات متعدد الأعضاء. |
| [getDataSource()](#getDataSource--) | يحصل على مصدر البيانات. |
| [getEnableCreateBindColumnHeader()](#getEnableCreateBindColumnHeader--) | في وضع ربط البيانات، يحدد ما إذا كان سيتم إنشاء عناوين رؤوس الأعمدة المرتبطة في الورقة. |
| [getIndex()](#getIndex--) | يحصل على الفهرس الخاص به داخل أوراق العمل. |
| [getName()](#getName--) | يحصل على اسم الورقة. |
| [getUniqueID()](#getUniqueID--) | يحصل على UniqueID في التحكم |
| [getValidations()](#getValidations--) | يحصل على مجموعة إعدادات التحقق من صحة البيانات في ورقة العمل. |
| [getVisible()](#getVisible--) | يشير إلى ما إذا كان اسم هذه الورقة معروضًا في علامات تبويب الورقة في التحكم. |
| [groupRows(int firstIndex, int lastIndex)](#groupRows-int-int-) | يقوم بتجميع الصفوف. |
| [groupRows(int firstIndex, int lastIndex, boolean isHidden)](#groupRows-int-int-boolean-) | يقوم بتجميع الصفوف. |
| [hashCode()](#hashCode--) |  |
| [isProtected()](#isProtected--) | يحصل على ما إذا كانت ورقة العمل محمية. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllCellsEditable()](#setAllCellsEditable--) | يجعل جميع الخلايا قابلة للتحرير. هذا سمة موسعة. |
| [setAllCellsReadonly()](#setAllCellsReadonly--) | يجعل جميع الخلايا للقراءة فقط. هذه سمة موسعة، لاحظ أن هذه السمة لا يمكن الاحتفاظ بها في الخلية الفعلية، إذا كنت تريد الحفاظ على الحماية يرجى استخدام setProtect. |
| [setBindStartColumn(int value)](#setBindStartColumn-int-) | في وضع ربط البيانات، يشير BindStartRow و BindStartColumn إلى موضع الشبكة للربط بمصدر البيانات. |
| [setBindStartRow(int value)](#setBindStartRow-int-) | في وضع ربط البيانات، يشير BindStartRow و BindStartColumn إلى موضع الشبكة للربط بمصدر البيانات. |
| [setCurrentBindRows(int value)](#setCurrentBindRows-int-) | يحصل على عدد الصفوف المرتبطة في وضع ربط البيانات. |
| [setDataMember(String value)](#setDataMember-java.lang.String-) | يضبط الـ DataMember من مصدر البيانات متعدد الأعضاء. |
| [setDataSource(Object value)](#setDataSource-java.lang.Object-) | يضبط مصدر البيانات. |
| [setEditableRange(int startRow, int startColumn, int rows, int columns)](#setEditableRange-int-int-int-int-) | يجعل نطاقًا من الخلايا قابلاً للتحرير. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells اجعل جميع الخلايا للقراءة فقط عن طريق استدعاء طريقة SetAllCellsReadonly. |
| [setEnableCreateBindColumnHeader(boolean value)](#setEnableCreateBindColumnHeader-boolean-) | في وضع ربط البيانات، يحدد ما إذا كان سيتم إنشاء عناوين رؤوس الأعمدة المرتبطة في الورقة. |
| [setName(String value)](#setName-java.lang.String-) | يضبط اسم الورقة. |
| [setProtected(boolean value)](#setProtected-boolean-) | يضبط ما إذا كانت ورقة العمل محمية. |
| [setReadonlyRange(int startRow, int startColumn, int rows, int columns)](#setReadonlyRange-int-int-int-int-) | يجعل نطاقًا من الخلايا للقراءة فقط. http://docs.aspose.com:8082/docs/display/cellsnet/Protecting+Cells أولاً اجعل جميع الخلايا قابلة للتحرير عن طريق استدعاء طريقة SetAllCellsEditable. |
| [setVisible(boolean value)](#setVisible-boolean-) | يشير إلى ما إذا كان اسم هذه الورقة معروضًا في علامات تبويب الورقة في التحكم. |
| [toString()](#toString--) |  |
| [unfreezePanes()](#unfreezePanes--) | يفك تجميد الألواح في ورقة العمل. |
| [ungroupRows(int firstIndex, int lastIndex)](#ungroupRows-int-int-) | يفك تجميع الصفوف. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### WorksheetDesign() {#WorksheetDesign--}
```
public WorksheetDesign()
```


المنشئ الافتراضي.

### WorksheetDesign(MainWeb mw, GridWorksheet gwk) {#WorksheetDesign-com.aspose.gridweb.MainWeb-com.aspose.gridweb.GridWorksheet-}
```
public WorksheetDesign(MainWeb mw, GridWorksheet gwk)
```


البناء مع MainWeb و GridWorksheet

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| mw | [MainWeb](../../com.aspose.gridweb/mainweb) |  |
| gwk | [GridWorksheet](../../com.aspose.gridweb/gridworksheet) |  |

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

### autoFitColumn(int columnIndex, int startRow, int endRow) {#autoFitColumn-int-int-int-}
```
public void autoFitColumn(int columnIndex, int startRow, int endRow)
```


يضبط عرض العمود تلقائيًا. تقوم هذه الطريقة بضبط عرض العمود تلقائيًا بناءً على المحتوى في نطاق من الخلايا داخل العمود من startRow إلى endRow. AutoFitColumn هي دالة غير دقيقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| columnIndex | int | فهرس العمود، يبدأ من الصفر |
| startRow | int | فهرس صف البداية، يبدأ من الصفر |
| endRow | int | فهرس صف النهاية، يبدأ من الصفر |

### cancelNewBindRow() {#cancelNewBindRow--}
```
public int cancelNewBindRow()
```


يلغي ويحذف الصف المرتبط المضاف حديثًا.

**Returns:**
int - فهرس الصف. إذا لم يتم إنشاء صف ربط جديد، يرجع -1.
### commitNewBindRow() {#commitNewBindRow--}
```
public int commitNewBindRow()
```


يؤكد الصف المرتبط المضاف حديثًا ويضيفه إلى مصدر البيانات.

**Returns:**
int - فهرس الصف الجديد. إذا لم يتم إنشاء صف، يرجع -1.
### copy(WebWorksheet source) {#copy-com.aspose.gridweb.WebWorksheet-}
```
public void copy(WebWorksheet source)
```


ينسخ من كائن ورقة عمل آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [WebWorksheet](../../com.aspose.gridweb/webworksheet) | الورقة الأخرى. |

### createAutoGenratedColumns() {#createAutoGenratedColumns--}
```
public void createAutoGenratedColumns()
```


بعد تعيين مصدر بيانات للورقة، استدعِ هذه الطريقة لتوليد الأعمدة المرتبطة تلقائيًا.

### createNewBindRow() {#createNewBindRow--}
```
public int createNewBindRow()
```


ينشئ صفًا مرتبطًا جديدًا ويربطه بمصدر البيانات.

**Returns:**
int - فهرس الصف الجديد. إذا لم يتم إنشاء صف، يرجع -1.
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

### dataBind() {#dataBind--}
```
public void dataBind()
```


اربط الورقة بمصدر البيانات.

### deleteBindRow(int rowNum) {#deleteBindRow-int-}
```
public int deleteBindRow(int rowNum)
```


يحذف صفًا مرتبطًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| rowNum | int | The row index. |

**Returns:**
int - فهرس الصف المحذوف. إذا لم يتم حذف صف ربط، يرجع -1.
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

### getBindStartColumn() {#getBindStartColumn--}
```
public int getBindStartColumn()
```


في وضع ربط البيانات، يشير BindStartRow و BindStartColumn إلى موضع الشبكة للربط بمصدر البيانات.

**Returns:**
int
### getBindStartRow() {#getBindStartRow--}
```
public int getBindStartRow()
```


في وضع ربط البيانات، يشير BindStartRow و BindStartColumn إلى موضع الشبكة للربط بمصدر البيانات.

**Returns:**
int
### getBindingSource() {#getBindingSource--}
```
public Iterable getBindingSource()
```


كائن مصدر البيانات المرتبط فعليًا في وقت التشغيل. يكون كائن DataView عندما تكون خاصية DataSource هي كائن DataSet أو DataTable أو DataView.

**Returns:**
java.lang.Iterable
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCurrentBindRows() {#getCurrentBindRows--}
```
public int getCurrentBindRows()
```


يحصل على عدد الصفوف المرتبطة في وضع ربط البيانات.

**Returns:**
int
### getDataMember() {#getDataMember--}
```
public String getDataMember()
```


يحصل على الـ DataMember من مصدر البيانات متعدد الأعضاء. عادةً ما يمثل كائن DataTable من DataSet.

**Returns:**
java.lang.String
### getDataSource() {#getDataSource--}
```
public Object getDataSource()
```


يحصل على مصدر البيانات. عادةً ما يكون كائن DataSet.

**Returns:**
java.lang.Object
### getEnableCreateBindColumnHeader() {#getEnableCreateBindColumnHeader--}
```
public boolean getEnableCreateBindColumnHeader()
```


في وضع ربط البيانات، يحدد ما إذا كان سيتم إنشاء عناوين رؤوس الأعمدة المرتبطة في الورقة.

**Returns:**
boolean
### getIndex() {#getIndex--}
```
public int getIndex()
```


يحصل على الفهرس الخاص به داخل أوراق العمل.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الورقة.

**Returns:**
java.lang.String
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
### groupRows(int firstIndex, int lastIndex) {#groupRows-int-int-}
```
public void groupRows(int firstIndex, int lastIndex)
```


يقوم بتجميع الصفوف.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول لتجميعه. |
| lastIndex | int | فهرس الصف الأخير لتجميعه. |

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
### isProtected() {#isProtected--}
```
public boolean isProtected()
```


يحصل على ما إذا كانت ورقة العمل محمية. عندما تكون ورقة العمل محمية، لا يمكن تحرير جميع الخلايا باستثناء الخلية التي تكون خاصية IsLocked فيها false.

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

### setBindStartColumn(int value) {#setBindStartColumn-int-}
```
public void setBindStartColumn(int value)
```


في وضع ربط البيانات، يشير BindStartRow و BindStartColumn إلى موضع الشبكة للربط بمصدر البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setBindStartRow(int value) {#setBindStartRow-int-}
```
public void setBindStartRow(int value)
```


في وضع ربط البيانات، يشير BindStartRow و BindStartColumn إلى موضع الشبكة للربط بمصدر البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setCurrentBindRows(int value) {#setCurrentBindRows-int-}
```
public void setCurrentBindRows(int value)
```


يحصل على عدد الصفوف المرتبطة في وضع ربط البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setDataMember(String value) {#setDataMember-java.lang.String-}
```
public void setDataMember(String value)
```


يضبط الـ DataMember من مصدر البيانات متعدد الأعضاء. عادةً ما يمثل كائن DataTable من DataSet.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setDataSource(Object value) {#setDataSource-java.lang.Object-}
```
public void setDataSource(Object value)
```


يضبط مصدر البيانات. عادةً ما يكون كائن DataSet.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

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

### setEnableCreateBindColumnHeader(boolean value) {#setEnableCreateBindColumnHeader-boolean-}
```
public void setEnableCreateBindColumnHeader(boolean value)
```


في وضع ربط البيانات، يحدد ما إذا كان سيتم إنشاء عناوين رؤوس الأعمدة المرتبطة في الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```


يضبط اسم الورقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setProtected(boolean value) {#setProtected-boolean-}
```
public void setProtected(boolean value)
```


يضبط ما إذا كانت ورقة العمل محمية. عندما تكون ورقة العمل محمية، لا يمكن تحرير جميع الخلايا باستثناء الخلية التي تكون خاصية IsLocked فيها false.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

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

### setVisible(boolean value) {#setVisible-boolean-}
```
public void setVisible(boolean value)
```


يشير إلى ما إذا كان اسم هذه الورقة معروضًا في علامات تبويب الورقة في التحكم.

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
### unfreezePanes() {#unfreezePanes--}
```
public void unfreezePanes()
```


يفك تجميد الألواح في ورقة العمل.

### ungroupRows(int firstIndex, int lastIndex) {#ungroupRows-int-int-}
```
public void ungroupRows(int firstIndex, int lastIndex)
```


يفك تجميع الصفوف.

**Remarks**

يزيل فقط معلومات المجموعة الخارجية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| firstIndex | int | فهرس الصف الأول الذي سيتم فك تجميعه. |
| lastIndex | int | فهرس الصف الأخير الذي سيتم فك تجميعه. |

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

