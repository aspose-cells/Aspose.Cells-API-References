---
title: "GridValidation"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل data validation.settings."
type: docs
url: /ar/java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

يمثل data validation.settings.
## حقول

| حقل | الوصف |
| --- | --- |
| [ServerValidation](#ServerValidation) | يحصل أو يضبط اسم دالة جافا سكريبت للتحقق من الصحة على جانب الخادم. |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | أضف إعدادات التحقق من الصحة في الخلية. |
| [addACell(String cellname)](#addACell-java.lang.String-) | أضف إعدادات التحقق من الصحة في الخلية. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | يطبق التحقق على المنطقة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | يمثل مجموعة من [GridCellArea](../../com.aspose.gridweb/gridcellarea) التي تحتوي على إعدادات التحقق من صحة البيانات. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | يحصل على اسم دالة جافا سكريبت للتحقق من الصحة على جانب العميل. |
| [getErrorMessage()](#getErrorMessage--) | يمثل رسالة خطأ التحقق من البيانات. |
| [getErrorTitle()](#getErrorTitle--) | يمثل عنوان مربع حوار خطأ التحقق من البيانات. |
| [getFormula1()](#getFormula1--) | يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات. |
| [getFormula2()](#getFormula2--) | يمثل القيمة أو التعبير المرتبط بالجزء الثاني من التحقق من صحة البيانات. |
| [getInputMessage()](#getInputMessage--) | يمثل رسالة خطأ التحقق من البيانات. |
| [getInputTitle()](#getInputTitle--) | يمثل عنوان مربع حوار إدخال التحقق من صحة البيانات. |
| [getListValue(int row, int column)](#getListValue-int-int-) | احصل على القيمة لقائمة التحقق للخلية المحددة. |
| [getOperator()](#getOperator--) | يمثل المشغل للتحقق من صحة البيانات. |
| [getRegEx()](#getRegEx--) | يحصل على سلسلة التعبير النمطي. |
| [getShowError()](#getShowError--) | يشير إلى ما إذا كانت رسالة خطأ التحقق من صحة البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة. |
| [getShowInput()](#getShowInput--) | يشير إلى ما إذا كانت رسالة إدخال التحقق من صحة البيانات ستُعرض كلما اختار المستخدم خلية في نطاق التحقق من صحة البيانات. |
| [getValidationType()](#getValidationType--) | يحصل على نوع التحقق من الصحة. |
| [getValue1()](#getValue1--) | يمثل القيمة المرتبطة بالتحقق من صحة البيانات. |
| [getValueList()](#getValueList--) | يحصل على كائن قائمة القيم. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | يحصل على ما إذا كانت قيمة الخلية مطلوبة. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | إزالة إعدادات التحقق في الخلية. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | إزالة إعدادات التحقق في النطاق. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | يضبط اسم دالة جافا سكريبت للتحقق من الصحة على جانب العميل. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | يمثل رسالة خطأ التحقق من البيانات. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | يمثل عنوان مربع حوار خطأ التحقق من البيانات. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | يمثل القيمة أو التعبير المرتبط بالجزء الثاني من التحقق من صحة البيانات. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | يمثل رسالة خطأ التحقق من البيانات. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | يمثل عنوان مربع حوار إدخال التحقق من صحة البيانات. |
| [setOperator(int value)](#setOperator-int-) | يمثل المشغل للتحقق من صحة البيانات. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | يضبط سلسلة التعبير النمطي. |
| [setRequired(boolean value)](#setRequired-boolean-) | يضبط ما إذا كانت قيمة الخلية مطلوبة. |
| [setShowError(boolean value)](#setShowError-boolean-) | يشير إلى ما إذا كانت رسالة خطأ التحقق من صحة البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | يشير إلى ما إذا كانت رسالة إدخال التحقق من صحة البيانات ستُعرض كلما اختار المستخدم خلية في نطاق التحقق من صحة البيانات. |
| [setValidationType(int value)](#setValidationType-int-) | يضبط نوع التحقق من الصحة. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | يضبط كائن قائمة القيم. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


يحصل أو يضبط اسم دالة جافا سكريبت للتحقق من الصحة على جانب الخادم.

**Remarks**

استخدم خاصية GridCustomServerValidation لتحديد التحقق من الصحة على جانب الخادم.

### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```


أضف إعدادات التحقق من الصحة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |

### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```


أضف إعدادات التحقق من الصحة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellname | java.lang.String | اسم الخلية. |

### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```


يطبق التحقق على المنطقة.

**Remarks**

في هذه الطريقة، سنقوم بإزالة جميع عمليات التحقق القديمة في هذه المنطقة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | المنطقة. |

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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```


يمثل مجموعة من [GridCellArea](../../com.aspose.gridweb/gridcellarea) التي تحتوي على إعدادات التحقق من صحة البيانات.

**Remarks**

التحققات القديمة على المنطقة لن تُزال إذا تم إضافة مباشرة إلى هذه القائمة.

**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```


يحصل على اسم دالة جافا سكريبت للتحقق من الصحة على جانب العميل.

**Remarks**

استخدم الخاصية ClientValidationFunction لتحديد اسم دالة التحقق من العميل. يجب إعلان الدالة بهذه الصيغة:
function customValicationFunction(source, value)
المعامل "source" هو كائن الخلية. المعامل "value" هو قيمة النص لخلية يتم فحصها. يجب أن تُرجع الدالة true إذا كانت القيمة صالحة.

**Returns:**
java.lang.String
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```


يمثل رسالة خطأ التحقق من البيانات.

**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```


يمثل عنوان مربع حوار خطأ التحقق من البيانات.

**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات.

**Returns:**
java.lang.String
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


يمثل القيمة أو التعبير المرتبط بالجزء الثاني من التحقق من صحة البيانات.

**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


يمثل رسالة خطأ التحقق من البيانات.

**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```


يمثل عنوان مربع حوار إدخال التحقق من صحة البيانات.

**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```


احصل على القيمة لقائمة التحقق للخلية المحددة.

**Remarks**

فقط للتحقق الذي يكون نوعه List وتم تطبيقه على الخلية المحددة، وإلا سيتم إرجاع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
java.lang.Object - القيمة لإنتاج قائمة هذا التحقق للخلية المحددة. إذا كانت القائمة تشير إلى نطاق، فإن القيمة المرجعة ستكون كائن ReferredArea؛ وإلا قد تكون القيمة المرجعة null أو object[] أو كائن بسيط.
### getOperator() {#getOperator--}
```
public int getOperator()
```


يمثل المشغل للتحقق من صحة البيانات.

انظر [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


يحصل على سلسلة التعبير النمطي.

**Returns:**
java.lang.String
### getShowError() {#getShowError--}
```
public boolean getShowError()
```


يشير إلى ما إذا كانت رسالة خطأ التحقق من صحة البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة.

**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```


يشير إلى ما إذا كانت رسالة إدخال التحقق من صحة البيانات ستُعرض كلما اختار المستخدم خلية في نطاق التحقق من صحة البيانات.

**Returns:**
boolean
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


يحصل على نوع التحقق من الصحة.

انظر [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```


يمثل القيمة المرتبطة بالتحقق من صحة البيانات.

**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```


يحصل على كائن قائمة القيم.

**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```


يحصل على ما إذا كانت قيمة الخلية مطلوبة.

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




### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```


إزالة إعدادات التحقق في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |

### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```


إزالة إعدادات التحقق في النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | النطاق الذي يحتوي على إعدادات التحقق من البيانات. |

### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```


يضبط اسم دالة جافا سكريبت للتحقق من الصحة على جانب العميل.

**Remarks**

استخدم الخاصية ClientValidationFunction لتحديد اسم دالة التحقق من العميل. يجب إعلان الدالة بهذه الصيغة:
function customValicationFunction(source, value)
المعامل "source" هو كائن الخلية. المعامل "value" هو قيمة النص لخلية يتم فحصها. يجب أن تُرجع الدالة true إذا كانت القيمة صالحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


يمثل رسالة خطأ التحقق من البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


يمثل عنوان مربع حوار خطأ التحقق من البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


يمثل القيمة أو التعبير المرتبط بالجزء الثاني من التحقق من صحة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


يمثل رسالة خطأ التحقق من البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


يمثل عنوان مربع حوار إدخال التحقق من صحة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


يمثل المشغل للتحقق من صحة البيانات.

انظر [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


يضبط سلسلة التعبير النمطي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


يضبط ما إذا كانت قيمة الخلية مطلوبة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


يشير إلى ما إذا كانت رسالة خطأ التحقق من صحة البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


يشير إلى ما إذا كانت رسالة إدخال التحقق من صحة البيانات ستُعرض كلما اختار المستخدم خلية في نطاق التحقق من صحة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


يضبط نوع التحقق من الصحة.

انظر [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


يضبط كائن قائمة القيم.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.util.ArrayList<java.lang.String> |  |

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

