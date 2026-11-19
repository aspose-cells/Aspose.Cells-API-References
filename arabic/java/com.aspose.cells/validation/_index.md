---
title: "التحقق"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل data validation.settings."
type: docs
url: /ar/java/com.aspose.cells/validation/
---

**Inheritance:**
java.lang.Object
```
public class Validation
```

يمثل data validation.settings.

**Example**

```
         Workbook workbook = new Workbook();
         	ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
         	CellArea area = CellArea.createCellArea(0, 0, 1, 1);
         	Validation validation = validations.get(validations.add(area));
         	validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
         	validation.setOperator(OperatorType.BETWEEN);
         	validation.setFormula1("3");
         	validation.setFormula2("1234");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | يطبق التحقق على المنطقة. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | يطبق التحقق على المنطقة. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | يطبق التحقق على المناطق المحددة. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | نسخ التحقق. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | يمثل نمط تنبيه التحقق. |
| [getAreas()](#getAreas--) | يحصل على جميع [CellArea](../../com.aspose.cells/cellarea) التي تحتوي على إعدادات التحقق من البيانات. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | يمثل رسالة خطأ التحقق من البيانات. |
| [getErrorTitle()](#getErrorTitle--) | يمثل عنوان مربع حوار خطأ التحقق من البيانات. |
| [getFormula1()](#getFormula1--) | يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | يحصل على القيمة أو التعبير المرتبط بهذا التحقق. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | يحصل على القيمة أو التعبير المرتبط بهذا التحقق للخلية المحددة. |
| [getFormula2()](#getFormula2--) | يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | يحصل على القيمة أو التعبير المرتبط بهذا التحقق. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | يحصل على القيمة أو التعبير المرتبط بهذا التحقق للخلية المحددة. |
| [getIgnoreBlank()](#getIgnoreBlank--) | يشير إلى ما إذا كانت القيم الفارغة مسموح بها بواسطة تحقق النطاق للبيانات. |
| [getInCellDropDown()](#getInCellDropDown--) | يشير إلى ما إذا كان التحقق من صحة البيانات يعرض قائمة منسدلة تحتوي على القيم المقبولة. |
| [getInputMessage()](#getInputMessage--) | يمثل رسالة إدخال التحقق من صحة البيانات. |
| [getInputTitle()](#getInputTitle--) | يمثل عنوان مربع حوار إدخال التحقق من صحة البيانات. |
| [getListValue(int row, int column)](#getListValue-int-int-) | احصل على القيمة لقائمة التحقق للخلية المحددة. |
| [getOperator()](#getOperator--) | يمثل المشغل للتحقق من صحة البيانات. |
| [getShowError()](#getShowError--) | يشير إلى ما إذا كانت رسالة خطأ التحقق من صحة البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة. |
| [getShowInput()](#getShowInput--) | يشير إلى ما إذا كانت رسالة إدخال التحقق من صحة البيانات ستُعرض كلما اختار المستخدم خلية في نطاق التحقق من صحة البيانات. |
| [getType()](#getType--) | يمثل نوع التحقق من صحة البيانات. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | احصل على قيمة التحقق في الخلية المحددة. |
| [getValue1()](#getValue1--) | يمثل القيمة الأولى المرتبطة بالتحقق من صحة البيانات. |
| [getValue2()](#getValue2--) | يمثل القيمة الثانية المرتبطة بالتحقق من صحة البيانات. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | إزالة إعدادات التحقق في الخلية. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | إزالة إعدادات التحقق في النطاق. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | يزيل هذا التحقق من المناطق المحددة. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | يمثل نمط تنبيه التحقق. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | يمثل رسالة خطأ التحقق من البيانات. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | يمثل عنوان مربع حوار خطأ التحقق من البيانات. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | يضبط القيمة أو التعبير المرتبط بهذا التحقق. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | يضبط القيمة أو التعبير المرتبط بهذا التحقق. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | يشير إلى ما إذا كانت القيم الفارغة مسموح بها بواسطة تحقق النطاق للبيانات. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | يشير إلى ما إذا كان التحقق من صحة البيانات يعرض قائمة منسدلة تحتوي على القيم المقبولة. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | يمثل رسالة إدخال التحقق من صحة البيانات. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | يمثل عنوان مربع حوار إدخال التحقق من صحة البيانات. |
| [setOperator(int value)](#setOperator-int-) | يمثل المشغل للتحقق من صحة البيانات. |
| [setShowError(boolean value)](#setShowError-boolean-) | يشير إلى ما إذا كانت رسالة خطأ التحقق من صحة البيانات ستُعرض كلما أدخل المستخدم بيانات غير صالحة. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | يشير إلى ما إذا كانت رسالة إدخال التحقق من صحة البيانات ستُعرض كلما اختار المستخدم خلية في نطاق التحقق من صحة البيانات. |
| [setType(int value)](#setType-int-) | يمثل نوع التحقق من صحة البيانات. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | يمثل القيمة الأولى المرتبطة بالتحقق من صحة البيانات. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | يمثل القيمة الثانية المرتبطة بالتحقق من صحة البيانات. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```


يطبق التحقق على المنطقة.

**Remarks**

إنه يعادل استخدام [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) مع فحص التقاطع والحافة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | المنطقة. |

### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```


يطبق التحقق على المنطقة.

**Remarks**

في هذه الطريقة، سنزيل جميع عمليات التحقق القديمة في المنطقة المحددة. بالنسبة للمدى العلوي الأيسر لتطبيقات التحقق، أولاً يكون StartRow هو الأصغر، ثانياً يكون StartColumn هو الأصغر بين تلك المناطق التي لها نفس أصغر StartRow.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | المنطقة. |
| checkIntersection | boolean | ما إذا كان يتم فحص تقاطع المنطقة المحددة مع مناطق عمليات التحقق الموجودة. إذا تم تطبيق عملية تحقق واحدة في المنطقة المحددة (أو جزء منها)، يجب إزالة عملية التحقق الموجودة أولاً من المنطقة المحددة. وإلا قد يحدث تلف في عمليات التحقق المولدة. إذا كان المستخدم متأكدًا من أن المنطقة المضافة لا تتقاطع مع أي منطقة موجودة، يمكن ضبط هذا المعامل كقيمة false لأغراض تحسين الأداء. |
| checkEdge | boolean | ما إذا كان يتم فحص حافة المناطق التي تم تطبيق هذا التحقق عليها. تعتمد الإعدادات الداخلية للتحقق على العنصر العلوي الأيسر من نطاقاته المطبقة، لذا إذا أصبحت المنطقة المحددة هي العنصر العلوي الأيسر الجديد للنطاقات المطبقة، يجب تعديل وإعادة بناء الإعدادات الداخلية، وإلا قد ينتج نتيجة غير متوقعة. إذا كان المستخدم متأكدًا من أن المنطقة المضافة ليست العنصر العلوي الأيسر، يمكن ضبط هذا المعامل كقيمة false لأغراض تحسين الأداء. |

### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```


يطبق التحقق على المناطق المحددة.

**Remarks**

في هذه الطريقة، سنزيل جميع عمليات التحقق القديمة في المنطقة المحددة. بالنسبة للمدى العلوي الأيسر لتطبيقات التحقق، أولاً يكون StartRow هو الأصغر، ثانياً يكون StartColumn هو الأصغر بين تلك المناطق التي لها نفس أصغر StartRow.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | المناطق. |
| checkIntersection | boolean | ما إذا كان يتم فحص تقاطع المنطقة المحددة مع مناطق عمليات التحقق الموجودة. إذا تم تطبيق عملية تحقق واحدة في المنطقة المحددة (أو جزء منها)، يجب إزالة عملية التحقق الموجودة أولاً من المنطقة المحددة. وإلا قد يحدث تلف في عمليات التحقق المولدة. إذا كان المستخدم متأكدًا من أن جميع المناطق المضافة لا تتقاطع مع أي منطقة موجودة، يمكن ضبط هذا المعامل كقيمة false لأغراض تحسين الأداء. |
| checkEdge | boolean | ما إذا كان يتم فحص حافة المناطق التي تم تطبيق هذا التحقق عليها. تعتمد الإعدادات الداخلية للتحقق على العنصر العلوي الأيسر من نطاقاته المطبقة، لذا إذا أصبحت إحدى المناطق المحددة هي العنصر العلوي الأيسر الجديد للنطاقات المطبقة، يجب تعديل وإعادة بناء الإعدادات الداخلية، وإلا قد ينتج نتيجة غير متوقعة. إذا كان المستخدم متأكدًا من أن لا واحدة من تلك المناطق المضافة هي العنصر العلوي الأيسر، يمكن ضبط هذا المعامل كقيمة false لأغراض تحسين الأداء. |

### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```


نسخ التحقق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | التحقق من المصدر. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | خيار النسخ. |

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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```


يمثل نمط تنبيه التحقق.

انظر [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```


يحصل على جميع [CellArea](../../com.aspose.cells/cellarea) التي تحتوي على إعدادات التحقق من البيانات.

**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


يحصل على القيمة أو التعبير المرتبط بهذا التحقق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - القيمة أو التعبير المرتبط بهذا التحقق.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


يحصل على القيمة أو التعبير المرتبط بهذا التحقق للخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
java.lang.String - القيمة أو التعبير المرتبط بهذا التحقق.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات.

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


يحصل على القيمة أو التعبير المرتبط بهذا التحقق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - القيمة أو التعبير المرتبط بهذا التحقق.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


يحصل على القيمة أو التعبير المرتبط بهذا التحقق للخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
java.lang.String - القيمة أو التعبير المرتبط بهذا التحقق.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```


يشير إلى ما إذا كانت القيم الفارغة مسموح بها بواسطة تحقق النطاق للبيانات.

**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```


يشير إلى ما إذا كان التحقق من صحة البيانات يعرض قائمة منسدلة تحتوي على القيم المقبولة.

**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```


يمثل رسالة إدخال التحقق من صحة البيانات.

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
java.lang.Object - القيمة لإنتاج قائمة هذا التحقق للخلية المحددة. إذا كانت القائمة تشير إلى نطاق، فستكون القيمة المرجعة كائنًا من نوع [ReferredArea](../../com.aspose.cells/referredarea)؛ وإلا قد تكون القيمة المرجعة null أو object[] أو كائن بسيط.
### getOperator() {#getOperator--}
```
public int getOperator()
```


يمثل المشغل للتحقق من صحة البيانات.

انظر [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
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
### getType() {#getType--}
```
public int getType()
```


يمثل نوع التحقق من صحة البيانات.

انظر [ValidationType](../../com.aspose.cells/validationtype).

**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```


احصل على قيمة التحقق في الخلية المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |
| isValue1 | boolean | يشير إلى ما إذا كان يتم الحصول على القيمة الأولى. |

**Returns:**
java.lang.Object - 
### getValue1() {#getValue1--}
```
public Object getValue1()
```


يمثل القيمة الأولى المرتبطة بالتحقق من صحة البيانات.

**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```


يمثل القيمة الثانية المرتبطة بالتحقق من صحة البيانات.

**Returns:**
java.lang.Object
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

### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```


إزالة إعدادات التحقق في النطاق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | المناطق التي يجب إزالة إعدادات هذا التحقق منها. |

### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```


يزيل هذا التحقق من المناطق المحددة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | المناطق التي يجب إزالة إعدادات هذا التحقق منها. |

### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```


يمثل نمط تنبيه التحقق.

انظر [ValidationAlertType](../../com.aspose.cells/validationalerttype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


يضبط القيمة أو التعبير المرتبط بهذا التحقق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| isR1C1 | boolean | ما إذا كانت الصيغة من نوع R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


يمثل القيمة أو التعبير المرتبط بالتحقق من البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


يضبط القيمة أو التعبير المرتبط بهذا التحقق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| isR1C1 | boolean | ما إذا كانت الصيغة من نوع R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |

### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```


يشير إلى ما إذا كانت القيم الفارغة مسموح بها بواسطة تحقق النطاق للبيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```


يشير إلى ما إذا كان التحقق من صحة البيانات يعرض قائمة منسدلة تحتوي على القيم المقبولة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


يمثل رسالة إدخال التحقق من صحة البيانات.

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

انظر [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

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

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يمثل نوع التحقق من صحة البيانات.

انظر [ValidationType](../../com.aspose.cells/validationtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```


يمثل القيمة الأولى المرتبطة بالتحقق من صحة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```


يمثل القيمة الثانية المرتبطة بالتحقق من صحة البيانات.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

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

