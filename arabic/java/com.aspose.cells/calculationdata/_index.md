---
title: "CalculationData"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل البيانات المطلوبة عند حساب دالة واحدة مثل معلمات اسم الدالة ... إلخ."
type: docs
url: /ar/java/com.aspose.cells/calculationdata/
---

**Inheritance:**
java.lang.Object
```
public class CalculationData
```

يمثل البيانات المطلوبة عند حساب دالة واحدة، مثل اسم الدالة، المعلمات، ... إلخ.

**Remarks**

جميع الكائنات التي توفرها هذه الفئة مخصصة لغرض "القراءة" فقط. يجب على المستخدم عدم تغيير أي بيانات في المصنف أثناء عملية حساب الصيغة، وإلا قد يحدث نتيجة غير متوقعة أو استثناء.
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | يحصل على القيمة المحسوبة لهذه الدالة. |
| [getCell()](#getCell--) | يحصل على كائن الخلية حيث توجد الدالة. |
| [getCellColumn()](#getCellColumn--) | يحصل على فهرس العمود للخلية التي توجد فيها الدالة. |
| [getCellRow()](#getCellRow--) | يحصل على فهرس الصف للخلية التي توجد فيها الدالة. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | يحصل على اسم الدالة التي سيتم حسابها. |
| [getParamCount()](#getParamCount--) | يحصل على عدد المعلمات |
| [getParamText(int index)](#getParamText-int-) | يحصل على النص الحرفي للمعلمة في الفهرس المحدد. |
| [getParamValue(int index)](#getParamValue-int-) | يحصل على كائن القيمة الممثلة للمعلمة في فهرس معين. |
| [getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)](#getParamValueInArrayMode-int-int-int-) | يحصل على قيمة (قيم) المعلمة في فهرس معين. |
| [getWorkbook()](#getWorkbook--) | يحصل على كائن المصنف (Workbook) حيث توجد الدالة. |
| [getWorksheet()](#getWorksheet--) | يحصل على كائن ورقة العمل (Worksheet) حيث توجد الدالة. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | يضبط القيمة المحسوبة لهذه الدالة. |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```


يحصل على القيمة المحسوبة لهذه الدالة.

**Remarks**

يجب على المستخدم ضبط هذه الخاصية في محرك الحساب المخصص الخاص به للوظائف التي يدعمها المحرك، وستُعاد القيمة المضبوطة عند الحصول على هذه الخاصية لاحقًا. قد تكون القيمة المضبوطة من الأنواع الممكنة لـ [Cell.getValue()](../../com.aspose.cells/cell\#getValue--)، أو مصفوفة من مثل هذه القيم، أو نطاق (Range)، أو اسم (Name)، أو ReferredArea. الحصول على هذه الخاصية قبل ضبط قيمة لها سيجعل الدالة تُحسب بواسطة محرك الحساب الافتراضي لـ Aspose.Cells ثم تُعاد القيمة المحسوبة (عادةً يجب أن تكون \#NAME? للوظائف المعرفة من قبل المستخدم).

**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public Cell getCell()
```


يحصل على كائن الخلية حيث توجد الدالة.

**Remarks**

عند حساب صيغة دون تعيينها إلى خلية، مثلًا باستخدام [Worksheet.calculateFormula(String,CalculationOptions)](../../com.aspose.cells/worksheet\#calculateFormula-String-CalculationOptions-)، سيتم حساب الصيغة كما لو تم تعيينها إلى الخلية A1، لذا فإن كلًا من [getCellRow()](../../com.aspose.cells/calculationdata\#getCellRow--) و [getCellColumn()](../../com.aspose.cells/calculationdata\#getCellColumn--) يساويان 0. ومع ذلك، قد لا تكون الخلية A1 في ورقة العمل قد تم إنشاءها. لذلك في مثل هذه الحالة ستكون هذه الخاصية فارغة (null).

**Returns:**
[Cell](../../com.aspose.cells/cell)
### getCellColumn() {#getCellColumn--}
```
public int getCellColumn()
```


يحصل على فهرس العمود للخلية التي توجد فيها الدالة.

**Returns:**
int
### getCellRow() {#getCellRow--}
```
public int getCellRow()
```


يحصل على فهرس الصف للخلية التي توجد فيها الدالة.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```


يحصل على اسم الدالة التي سيتم حسابها.

**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```


يحصل على عدد المعلمات

**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```


يحصل على النص الحرفي للمعلمة في الفهرس المحدد.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس المعلمة (بدءًا من 0) |

**Returns:**
java.lang.String - النص الحرفي للمعلمة
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```


يحصل على كائن القيمة الممثلة للمعلمة في فهرس معين.

**Remarks**

لمعلمة واحدة:

إذا كانت قيمة عادية، فستُرجع القيمة العادية نفسها؛

إذا كانت إشارة، فستُرجع كائن ReferredArea؛

إذا كانت تشير إلى مجموعة بيانات (مجموعات) ذات قيم متعددة، فستُرجع مصفوفة من الكائنات؛

إذا كانت نوعًا من التعبير يحتاج إلى حساب، فسيتم حسابه في وضع القيمة وعادةً ما تُرجع قيمة واحدة وفقًا لخلية الأساس الحالية. على سبيل المثال، إذا كان أحد معلمات صيغة D2 هو A:A+B:B، فسيتم حساب A2+B2 وإرجاعه. ومع ذلك، إذا تم تحديد هذه المعلمة في وضع المصفوفة (عن طريق  أو )، فستُرجع مصفوفة (object[][]) تكون عناصرها A1+B1، A2+B2، ....

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس المعلمة (بدءًا من 0) |

**Returns:**
java.lang.Object - القيمة المحسوبة للمعلمة.
### getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount) {#getParamValueInArrayMode-int-int-int-}
```
public Object[][] getParamValueInArrayMode(int index, int maxRowCount, int maxColumnCount)
```


يحصل على قيمة (قيم) المعلمة في فهرس معين. إذا كانت المعلمة نوعًا من التعبير يحتاج إلى حساب، فسيتم حسابه في وضع المصفوة.

**Remarks**

للتعبير الذي يحتاج إلى حساب، مع أخذ A:A+B:B كمثال: في وضع القيمة سيُحسب إلى قيمة واحدة وفقًا لخلية الأساس الحالية. ولكن في وضع المصفوفة، سيتم حساب جميع قيم A1+B1، A2+B2، A3+B3، ... واستخدامها لإنشاء المصفوفة المرجعة. وفي مثل هذه الحالة، من الأفضل تحديد حد لعدد الصفوف/الأعمدة (مثلًا وفقًا لـ [Cells.getMaxDataRow()](../../com.aspose.cells/cells\#getMaxDataRow--) و [Cells.getMaxDataColumn()](../../com.aspose.cells/cells\#getMaxDataColumn--))، وإلا قد تزيد المصفوفة الكبيرة المرجعة من استهلاك الذاكرة بسبب كمية كبيرة من البيانات غير المفيدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| الفهرس | int | فهرس المعلمة (بدءًا من 0) |
| maxRowCount | int | حد عدد الصفوف للمصفوفة المرجعة. إذا كان غير إيجابي أو أكبر من عدد الصفوف الفعلي، فسيُستخدم عدد الصفوف الفعلي. |
| maxColumnCount | int | حد عدد الأعمدة للمصفوفة المرجعة. إذا كان غير إيجابي أو أكبر من عدد الصفوف الفعلي، فسيُستخدم عدد الأعمدة الفعلي. |

**Returns:**
java.lang.Object[][] - مصفوفة تحتوي على جميع العناصر التي يمثلها المعامل المحدد.
### getWorkbook() {#getWorkbook--}
```
public Workbook getWorkbook()
```


يحصل على كائن المصنف (Workbook) حيث توجد الدالة.

**Returns:**
[Workbook](../../com.aspose.cells/workbook)
### getWorksheet() {#getWorksheet--}
```
public Worksheet getWorksheet()
```


يحصل على كائن ورقة العمل (Worksheet) حيث توجد الدالة.

**Returns:**
[Worksheet](../../com.aspose.cells/worksheet)
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




### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```


يضبط القيمة المحسوبة لهذه الدالة.

**Remarks**

يجب على المستخدم ضبط هذه الخاصية في محرك الحساب المخصص الخاص به للوظائف التي يدعمها المحرك، وستُعاد القيمة المضبوطة عند الحصول على هذه الخاصية لاحقًا. قد تكون القيمة المضبوطة من الأنواع الممكنة لـ [Cell.getValue()](../../com.aspose.cells/cell\#getValue--)، أو مصفوفة من مثل هذه القيم، أو نطاق (Range)، أو اسم (Name)، أو ReferredArea. الحصول على هذه الخاصية قبل ضبط قيمة لها سيجعل الدالة تُحسب بواسطة محرك الحساب الافتراضي لـ Aspose.Cells ثم تُعاد القيمة المحسوبة (عادةً يجب أن تكون \#NAME? للوظائف المعرفة من قبل المستخدم).

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

