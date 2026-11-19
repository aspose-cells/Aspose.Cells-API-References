---
title: "GridCell"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل كائن خلية."
type: docs
url: /ar/java/com.aspose.gridweb/gridcell/
---

**Inheritance:**
java.lang.Object
```
public class GridCell
```

يمثل كائن خلية.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | ينسخ البيانات من خلية المصدر. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | انسخ النمط وضع النمط للخلية |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | ينشئ كائن تعليق للخلية. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | ينشئ كائن تحقق للخلية. |
| [equals(Object obj)](#equals-java.lang.Object-) | يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر. |
| [getBoolValue()](#getBoolValue--) | يحصل على القيمة المنطقية الموجودة في الخلية. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | يحصل على رقم العمود (بدءًا من الصفر) للخلية. |
| [getComment()](#getComment--) | احصل على كائن التعليق في هذه الخلية |
| [getDateValue()](#getDateValue--) | يحصل على قيمة DateTime الموجودة في الخلية. |
| [getDisplayStringValue()](#getDisplayStringValue--) | يحصل على قيمة السلسلة المنسقة لهذه الخلية. |
| [getDoubleValue()](#getDoubleValue--) | يحصل على القيمة المزدوجة الموجودة في الخلية. |
| [getFloatValue()](#getFloatValue--) | يحصل على القيمة العائمة الموجودة في الخلية. |
| [getFormula()](#getFormula--) | يحصل على صيغة من [GridCell](../../com.aspose.gridweb/gridcell). |
| [getHtmlString()](#getHtmlString--) | يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [getIntValue()](#getIntValue--) | يحصل على القيمة الصحيحة الموجودة في الخلية. |
| [getName()](#getName--) | يحصل على اسم الخلية. |
| [getRow()](#getRow--) | يحصل على رقم الصف (مبني على الصفر) للخلية. |
| [getStringValue()](#getStringValue--) | يحصل على القيمة النصية الموجودة في الخلية. |
| [getStyle()](#getStyle--) | يحصل على نسخة من نمط الخلية. ضع النمط للخلية. |
| [getType()](#getType--) | أرجع نوع قيمة الخلية، يمكن الاطلاع على المعنى في GridCellValueType.java |
| [getValue()](#getValue--) | يحصل على القيمة الموجودة في هذه الخلية. |
| [getWidthOfValue()](#getWidthOfValue--) | يحصل على عرض القيمة بوحدة البكسل. |
| [hashCode()](#hashCode--) | يعمل كدالة تجزئة لنوع معين. |
| [isErrorValue()](#isErrorValue--) | يتحقق مما إذا كانت الصيغة يمكنها تقييم النتيجة بشكل صحيح. |
| [isFormula()](#isFormula--) | يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة. |
| [isStyleSet()](#isStyleSet--) | يشير إلى ما إذا تم تعيين نمط الخلية. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | يضع قيمة منطقية في الخلية. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | يضع قيمة تاريخ/وقت في الخلية. |
| [putValue(double param_double)](#putValue-double-) | يضع قيمة مزدوجة في الخلية. |
| [putValue(int param_int)](#putValue-int-) | يضع قيمة عددية صحيحة في الخلية. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | يضع قيمة كائن في الخلية. نفس setValue(Object param\_object) |
| [putValue(String param_string)](#putValue-java.lang.String-) | يضع قيمة سلسلة في الخلية. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | يضع قيمة نصية في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | يضع قيمة في الخلية، وإذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة تعيين تنسيق الأرقام للخلية. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | يضبط قيمة الخلية بقيمة سلسلة ويضبط تنسيق الخلية بناءً على هذه القيمة. |
| [removeComment()](#removeComment--) | يزيل كائن التعليق للخلية. |
| [removeValidation()](#removeValidation--) | يزيل كائن التحقق للخلية. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | يضبط حدود (أعلى، أسفل، يسار ويمين) للخلية، جميع الحدود لها نفس نمط الحدود. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | يضبط التنسيق المخصص، القيمة null أو السلسلة الفارغة تعني عدم وجود تنسيق مخصص. |
| [setFormula(String value)](#setFormula-java.lang.String-) | يضبط صيغة للـ [GridCell](../../com.aspose.gridweb/gridcell). |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | اضبط الصيغة وقيمة الصيغة. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | يضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية. |
| [setNumberType(int numbertype)](#setNumberType-int-) | اضبط تنسيق العرض للأرقام والتواريخ |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | يحصل على نسخة من نمط الخلية. ضع النمط للخلية. |
| [setValue(Object value)](#setValue-java.lang.Object-) | يحصل على القيمة الموجودة في هذه الخلية. |
| [toString()](#toString--) | يرجع سلسلة تمثل كائن Cell الحالي. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```


يشير إلى ما إذا كانت هذه الخلية تحتوي على رابط خارجي. ينطبق فقط عندما تكون الخلية خلية صيغة.

**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```


ينسخ البيانات من خلية المصدر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | كائن المصدر [GridCell](../../com.aspose.gridweb/gridcell). |

### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```


انسخ النمط وضع النمط للخلية

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | نمط المصدر. |

### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```


ينشئ كائن تعليق للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| ملاحظة | java.lang.String | ملاحظة التعليق. |
| المؤلف | java.lang.String | مؤلف التعليق. |
| isvisible | boolean | ما إذا كان التعليق مرئياً. |

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```


ينشئ كائن تحقق للخلية.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
         		// Sets to number validation expression.
         		v.setRegEx("\\d+");
```

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). نوع التحقق. |
| isRequried | boolean | ما إذا كانت قيمة الخلية مطلوبة. |

**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - 
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```


يتحقق مما إذا كان هذا الكائن يشير إلى نفس الخلية مع كائن خلية آخر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| obj | java.lang.Object | كائن GridCell آخر |

**Returns:**
منطقي - true إذا كان كائنان خلية يشيران إلى نفس الخلية.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```


يحصل على القيمة المنطقية الموجودة في الخلية.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```


يحصل على رقم العمود (بدءًا من الصفر) للخلية.

**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```


احصل على كائن التعليق في هذه الخلية

**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```


يحصل على قيمة DateTime الموجودة في الخلية.

**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```


يحصل على قيمة السلسلة المنسقة لهذه الخلية.

**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```


يحصل على القيمة المزدوجة الموجودة في الخلية.

**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```


يحصل على القيمة العائمة الموجودة في الخلية.

**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```


يحصل على صيغة من [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

دائمًا ما يبدأ نص الصيغة بعلامة مساواة (=). ويرجى دائمًا استخدام الفاصلة (,) كفاصل للمعاملات، مثل "=SUM(A1, E1, H2)".

يمكن للمستخدم ضبط أي صيغة في ملف مصمم المصنف. ستحتفظ Aspose.Cells بجميع الصيغ. إذا استخدم المستخدم هذه الخاصية لتعيين صيغة لخلية، فإن الجزء الأكبر من الدوال المدمجة في المصنف مدعوم. والمزيد قادم. إذا كان لديك أي احتياج خاص لدوال المصنف المدمجة، يرجى إبلاغنا.

**Example**

```
         GridWeb GridWeb1 = new GridWeb();
         GridWorksheet sheet = GridWeb1.getActiveSheet();
         sheet.getCells().get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```

**Returns:**
java.lang.String
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```


يحصل على سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية.

**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```


يحصل على القيمة الصحيحة الموجودة في الخلية.

**Returns:**
int
### getName() {#getName--}
```
public String getName()
```


يحصل على اسم الخلية. على سبيل المثال: A1, F102.

**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```


يحصل على رقم الصف (مبني على الصفر) للخلية.

**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```


يحصل على القيمة النصية الموجودة في الخلية.

**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```


يحصل على نسخة من نمط الخلية. ضع النمط للخلية.

**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```


أرجع نوع قيمة الخلية، يمكن الاطلاع على المعنى في GridCellValueType.java

**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```


يحصل على القيمة الموجودة في هذه الخلية.

**Remarks**

النوع المحتمل:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```


يحصل على عرض القيمة بوحدة البكسل.

**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```


يعمل كدالة تجزئة لنوع معين.

**Returns:**
int - رمز تجزئة لكائن GridCell الحالي.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```


يتحقق مما إذا كانت الصيغة يمكنها تقييم النتيجة بشكل صحيح.

**Remarks**

ينطبق فقط على خلية الصيغة.

**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```


يمثل ما إذا كانت الخلية المحددة تحتوي على صيغة.

**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```


يشير إلى ما إذا كان نمط الخلية مضبوطًا. إذا تم إرجاع false، فهذا يعني أن هذه الخلية لها تنسيق خلية افتراضي.

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




### putValue(boolean param_boolean) {#putValue-boolean-}
```
public void putValue(boolean param_boolean)
```


يضع قيمة منطقية في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| param_boolean | boolean | قيمة الإدخال |

### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```


يضع قيمة تاريخ/وقت في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | قيمة الإدخال |

### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```


يضع قيمة مزدوجة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| param_double | double | قيمة الإدخال |

### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```


يضع قيمة عددية صحيحة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| param_int | int | قيمة الإدخال |

### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```


يضع قيمة كائن في الخلية. نفس setValue(Object param\_object)

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| objectValue | java.lang.Object | قيمة الإدخال |

### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```


يضع قيمة سلسلة في الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| param_string | java.lang.String | قيمة الإدخال |

### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```


يضع قيمة نصية في الخلية ويحول القيمة إلى نوع بيانات آخر إذا كان ذلك مناسبًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | java.lang.String | قيمة الإدخال |
| isConverted | boolean | True: تم التحويل إلى نوع بيانات آخر إذا كان مناسبًا. |

### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```


يضع قيمة في الخلية، وإذا كان مناسبًا سيتم تحويل القيمة إلى نوع بيانات آخر وسيتم إعادة تعيين تنسيق الأرقام للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | java.lang.String | قيمة الإدخال |
| isConverted | boolean | True: تم التحويل إلى نوع بيانات آخر إذا كان مناسبًا. |
| setStyle | boolean | True: ضبط تنسيق الرقم على نمط الخلية عند التحويل إلى نوع بيانات آخر |

### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```


يضبط قيمة الخلية بقيمة سلسلة ويضبط تنسيق الخلية بناءً على هذه القيمة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| stringValue | java.lang.String | قيمة الإدخال. |

### removeComment() {#removeComment--}
```
public void removeComment()
```


يزيل كائن التعليق للخلية.

### removeValidation() {#removeValidation--}
```
public void removeValidation()
```


يزيل كائن التحقق للخلية.

### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```


يضبط حدود (أعلى، أسفل، يسار ويمين) للخلية، جميع الحدود لها نفس نمط الحدود.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | نمط الحد. |

### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```


يضبط التنسيق المخصص، القيمة null أو السلسلة الفارغة تعني عدم وجود تنسيق مخصص.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| مخصص | java.lang.String | العرض المخصص للسلسلة |

### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```


يضبط صيغة للـ [GridCell](../../com.aspose.gridweb/gridcell).

**Remarks**

دائمًا ما يبدأ نص الصيغة بعلامة مساواة (=). ويرجى دائمًا استخدام الفاصلة (,) كفاصل للمعاملات، مثل "=SUM(A1, E1, H2)".

يمكن للمستخدم ضبط أي صيغة في ملف مصمم المصنف. ستحتفظ Aspose.Cells بجميع الصيغ. إذا استخدم المستخدم هذه الخاصية لتعيين صيغة لخلية، فإن الجزء الأكبر من الدوال المدمجة في المصنف مدعوم. والمزيد قادم. إذا كان لديك أي احتياج خاص لدوال المصنف المدمجة، يرجى إبلاغنا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```


اضبط الصيغة وقيمة الصيغة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | الصيغة. |
| القيمة | java.lang.Object | قيمة الصيغة. |

### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```


يضبط سلسلة HTML التي تحتوي على البيانات وبعض التنسيقات في هذه الخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```


اضبط تنسيق العرض للأرقام والتواريخ

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| numbertype | int | قيمة نوع الرقم، انظر GridTableItemStyle.NumberType |

### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```


يحصل على نسخة من نمط الخلية. ضع النمط للخلية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |

### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```


يحصل على القيمة الموجودة في هذه الخلية.

**Remarks**

النوع المحتمل:

null,

Boolean,

DateTime,

Double,

Integer

String.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.Object |  |

### toString() {#toString--}
```
public String toString()
```


يرجع سلسلة تمثل كائن Cell الحالي.

**Returns:**
java.lang.String -
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

