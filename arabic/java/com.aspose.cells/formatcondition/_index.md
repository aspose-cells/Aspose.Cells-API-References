---
title: "FormatCondition"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل شرط تنسيق شرطي."
type: docs
url: /ar/java/com.aspose.cells/formatcondition/
---

**Inheritance:**
java.lang.Object
```
public class FormatCondition
```

يمثل شرط تنسيق شرطي.

**Example**

```
         //Instantiating a Workbook object
         Workbook workbook = new Workbook();
         Worksheet sheet = workbook.getWorksheets().get(0);
 
         //Adds an empty conditional formatting
         int index = sheet.getConditionalFormattings().add();
         FormatConditionCollection fcs = sheet.getConditionalFormattings().get(index);
 
         //Sets the conditional format range.
         CellArea ca = new CellArea();
         ca.StartRow = 0;
         ca.EndRow = 0;
         ca.StartColumn = 0;
         ca.EndColumn = 0;
         fcs.addArea(ca);
 
         ca = new CellArea();
         ca.StartRow = 1;
         ca.EndRow = 1;
         ca.StartColumn = 1;
         ca.EndColumn = 1;
         fcs.addArea(ca);
 
         //Adds condition.
         int conditionIndex = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "=A2", "100");
 
         //Adds condition.
         int conditionIndex2 = fcs.addCondition(FormatConditionType.CELL_VALUE, OperatorType.BETWEEN, "50", "100");
 
         //Sets the background color.
         FormatCondition fc = fcs.get(conditionIndex);
         fc.getStyle().setBackgroundColor(Color.getRed());
 
         //Saving the Excel file
         workbook.save("output.xls");
```
## الطرق

| طريقة | الوصف |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAboveAverage()](#getAboveAverage--) | احصل على نسخة "AboveAverage" للتنسيق الشرطي. |
| [getClass()](#getClass--) |  |
| [getColorScale()](#getColorScale--) | احصل على نسخة "ColorScale" للتنسيق الشرطي. |
| [getDataBar()](#getDataBar--) | احصل على نسخة "DataBar" للتنسيق الشرطي. |
| [getFormula1()](#getFormula1--) | يحصل على القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | يحصل على القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | يحصل على القيمة أو التعبير لتنسيق الخلية الشرطي. |
| [getFormula1(int row, int column)](#getFormula1-int-int-) | يحصل على الصيغة لتنسيق الخلية الشرطي. |
| [getFormula2()](#getFormula2--) | يحصل على القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | يحصل على القيمة أو التعبير المرتبط بشرط التنسيق هذا. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | يحصل على القيمة أو التعبير لتنسيق الخلية الشرطي. |
| [getFormula2(int row, int column)](#getFormula2-int-int-) | يحصل على الصيغة لتنسيق الخلية الشرطي. |
| [getIconSet()](#getIconSet--) | احصل على نسخة "IconSet" للتنسيق الشرطي. |
| [getOperator()](#getOperator--) | يحصل على نوع عامل تنسيق الشرطي. |
| [getPriority()](#getPriority--) | أولوية قاعدة التنسيق الشرطي هذه. |
| [getStopIfTrue()](#getStopIfTrue--) | True، لا يمكن تطبيق قواعد ذات أولوية أقل على هذه القاعدة عندما تُقيم هذه القاعدة إلى true. |
| [getStyle()](#getStyle--) | يحصل أو يضبط نمط نطاقات الخلايا المُنسقة شرطياً. |
| [getText()](#getText--) | القيمة النصية في قاعدة تنسيق شرطي "text contains". |
| [getTimePeriod()](#getTimePeriod--) | الفترة الزمنية المتاحة في قاعدة تنسيق شرطي "date occurrin". |
| [getTop10()](#getTop10--) | احصل على نسخة "Top10" من التنسيق الشرطي. |
| [getType()](#getType--) | يحصل على ما إذا كان نوع التنسيق الشرطي. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | يضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | يضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| [setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)](#setFormulas-java.lang.String-java.lang.String-boolean-boolean-) | يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. |
| [setOperator(int value)](#setOperator-int-) | يضبط نوع عامل التنسيق الشرطي. |
| [setPriority(int value)](#setPriority-int-) | أولوية قاعدة التنسيق الشرطي هذه. |
| [setStopIfTrue(boolean value)](#setStopIfTrue-boolean-) | True، لا يمكن تطبيق قواعد ذات أولوية أقل على هذه القاعدة عندما تُقيم هذه القاعدة إلى true. |
| [setStyle(Style value)](#setStyle-com.aspose.cells.Style-) | يحصل أو يضبط نمط نطاقات الخلايا المُنسقة شرطياً. |
| [setText(String value)](#setText-java.lang.String-) | القيمة النصية في قاعدة تنسيق شرطي "text contains". |
| [setTimePeriod(int value)](#setTimePeriod-int-) | الفترة الزمنية المتاحة في قاعدة تنسيق شرطي "date occurrin". |
| [setType(int value)](#setType-int-) | يضبط ما إذا كان نوع التنسيق الشرطي. |
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
### getAboveAverage() {#getAboveAverage--}
```
public AboveAverage getAboveAverage()
```


احصل على نسخة "AboveAverage" من التنسيق الشرطي. القاعدة الافتراضية للنسخة تبرز الخلايا التي تتجاوز المتوسط لجميع القيم في النطاق. صالح فقط للنوع = AboveAverage.

**Returns:**
[AboveAverage](../../com.aspose.cells/aboveaverage) - 
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColorScale() {#getColorScale--}
```
public ColorScale getColorScale()
```


احصل على نسخة "ColorScale" من التنسيق الشرطي. النسخة الافتراضية هي مقياس ألوان "green-yellow-red" من نوع 3ColorScale. صالح فقط للنوع = ColorScale.

**Returns:**
[ColorScale](../../com.aspose.cells/colorscale) - 
### getDataBar() {#getDataBar--}
```
public DataBar getDataBar()
```


احصل على نسخة "DataBar" من التنسيق الشرطي. لون النسخة الافتراضية هو أزرق. صالح فقط للنوع = DataBar.

**Returns:**
[DataBar](../../com.aspose.cells/databar) - 
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```


يحصل على القيمة أو التعبير المرتبط بالتنسيق الشرطي.

**Remarks**

يرجى إضافة جميع المناطق قبل تعيين الصيغة. لتعيين صيغة لهذا الشرط، إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فستُعامل كقيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\\"=...\\"".

**Returns:**
java.lang.String
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```


يحصل على القيمة أو التعبير المرتبط بشرط التنسيق هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - القيمة أو التعبير المرتبط بهذا الشرط التنسيقي.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```


يحصل على القيمة أو التعبير لتنسيق الخلية الشرطي.

**Remarks**

يجب أن تكون الخلية المعطاة ضمن هذا التنسيق الشرطي، وإلا سيتم إرجاع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
java.lang.String - القيمة أو التعبير المرتبط بالتنسيق الشرطي للخلية.
### getFormula1(int row, int column) {#getFormula1-int-int-}
```
public String getFormula1(int row, int column)
```


يحصل على الصيغة لتنسيق الخلية الشرطي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
java.lang.String - الصيغة.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```


يحصل على القيمة أو التعبير المرتبط بالتنسيق الشرطي.

**Remarks**

يرجى إضافة جميع المناطق قبل تعيين الصيغة. لتعيين صيغة لهذا الشرط، إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فستُعامل كقيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\\"=...\\"".

**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```


يحصل على القيمة أو التعبير المرتبط بشرط التنسيق هذا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |

**Returns:**
java.lang.String - القيمة أو التعبير المرتبط بهذا الشرط التنسيقي.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```


يحصل على القيمة أو التعبير لتنسيق الخلية الشرطي.

**Remarks**

يجب أن تكون الخلية المعطاة ضمن هذا التنسيق الشرطي، وإلا سيتم إرجاع null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| isR1C1 | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق كـ R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة تحتاج إلى تنسيق حسب الإعدادات الإقليمية. |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
java.lang.String - القيمة أو التعبير المرتبط بالتنسيق الشرطي للخلية.
### getFormula2(int row, int column) {#getFormula2-int-int-}
```
public String getFormula2(int row, int column)
```


يحصل على الصيغة لتنسيق الخلية الشرطي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| صف | int | The row index. |
| عمود | int | The column index. |

**Returns:**
java.lang.String - الصيغة.
### getIconSet() {#getIconSet--}
```
public IconSet getIconSet()
```


احصل على نسخة "IconSet" من التنسيق الشرطي. نوع IconSetType للنسخة الافتراضية هو TrafficLights31. صالح فقط للنوع = IconSet.

**Returns:**
[IconSet](../../com.aspose.cells/iconset) - 
### getOperator() {#getOperator--}
```
public int getOperator()
```


يحصل على نوع عامل تنسيق الشرطي.

انظر [OperatorType](../../com.aspose.cells/operatortype).

**Returns:**
int
### getPriority() {#getPriority--}
```
public int getPriority()
```


أولوية قاعدة التنسيق الشرطي هذه. تُستخدم هذه القيمة لتحديد أي تنسيق يجب تقييمه وعرضه. القيم الرقمية الأقل لها أولوية أعلى من القيم الرقمية الأعلى، حيث أن '1' هي الأعلى أولوية.

**Returns:**
int
### getStopIfTrue() {#getStopIfTrue--}
```
public boolean getStopIfTrue()
```


True، لا يمكن تطبيق قواعد ذات أولوية أقل على هذه القاعدة عندما تُقيم هذه القاعدة إلى true. ينطبق فقط على Excel 2007؛

**Returns:**
boolean
### getStyle() {#getStyle--}
```
public Style getStyle()
```


يحصل أو يضبط نمط نطاقات الخلايا المُنسقة شرطياً.

**Returns:**
[Style](../../com.aspose.cells/style)
### getText() {#getText--}
```
public String getText()
```


القيمة النصية في قاعدة تنسيق شرطي "text contains". صالح فقط للنوع = containsText، notContainsText، beginsWith و endsWith. القيمة الافتراضية هي null.

**Returns:**
java.lang.String
### getTimePeriod() {#getTimePeriod--}
```
public int getTimePeriod()
```


الفترة الزمنية المتاحة في قاعدة تنسيق شرطي "date occurrin". صالح فقط للنوع = timePeriod. القيمة الافتراضية هي TimePeriodType.Today.

انظر [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Returns:**
int
### getTop10() {#getTop10--}
```
public Top10 getTop10()
```


احصل على نسخة "Top10" من التنسيق الشرطي. القاعدة الافتراضية للنسخة تبرز الخلايا التي تقع قيمها ضمن أعلى 10 نطاقات. صالح فقط للنوع = Top10.

**Returns:**
[Top10](../../com.aspose.cells/top10) - 
### getType() {#getType--}
```
public int getType()
```


يحصل على ما إذا كان نوع التنسيق الشرطي.

انظر [FormatConditionType](../../com.aspose.cells/formatconditiontype).

**Returns:**
int
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




### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


يضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي.

**Remarks**

يرجى إضافة جميع المناطق قبل تعيين الصيغة. لتعيين صيغة لهذا الشرط، إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فستُعامل كقيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\\"=...\\"".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```


يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فسيتم اعتبارها قيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\\"=...\\"". |
| isR1C1 | boolean | ما إذا كانت الصيغة من نوع R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


يضبط القيمة أو التعبير المرتبط بالتنسيق الشرطي.

**Remarks**

يرجى إضافة جميع المناطق قبل تعيين الصيغة. لتعيين صيغة لهذا الشرط، إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فستُعامل كقيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\\"=...\\"".

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```


يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula | java.lang.String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فسيتم اعتبارها قيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\\"=...\\"". |
| isR1C1 | boolean | ما إذا كانت الصيغة من نوع R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |

### setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal) {#setFormulas-java.lang.String-java.lang.String-boolean-boolean-}
```
public void setFormulas(String formula1, String formula2, boolean isR1C1, boolean isLocal)
```


يضبط القيمة أو التعبير المرتبط بهذا الشرط التنسيقي.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| formula1 | java.lang.String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. إذا بدأت القيمة المدخلة بـ '=', فسيتم اعتبارها صيغة. وإلا فسيتم اعتبارها قيمة عادية (نص، رقم، منطق). بالنسبة للقيمة النصية التي تبدأ بـ '=', يمكن للمستخدم إدخالها كصيغة بالتنسيق: "=\\"=...\\"". |
| formula2 | java.lang.String | القيمة أو التعبير المرتبط بهذا الشرط التنسيقي. تنسيق الإدخال هو نفسه مع formula1 |
| isR1C1 | boolean | ما إذا كانت الصيغة من نوع R1C1. |
| isLocal | boolean | ما إذا كانت الصيغة مهيأة وفقًا للمنطقة. |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


يضبط نوع عامل التنسيق الشرطي.

انظر [OperatorType](../../com.aspose.cells/operatortype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setPriority(int value) {#setPriority-int-}
```
public void setPriority(int value)
```


أولوية قاعدة التنسيق الشرطي هذه. تُستخدم هذه القيمة لتحديد أي تنسيق يجب تقييمه وعرضه. القيم الرقمية الأقل لها أولوية أعلى من القيم الرقمية الأعلى، حيث أن '1' هي الأعلى أولوية.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setStopIfTrue(boolean value) {#setStopIfTrue-boolean-}
```
public void setStopIfTrue(boolean value)
```


True، لا يمكن تطبيق قواعد ذات أولوية أقل على هذه القاعدة عندما تُقيم هذه القاعدة إلى true. ينطبق فقط على Excel 2007؛

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | boolean |  |

### setStyle(Style value) {#setStyle-com.aspose.cells.Style-}
```
public void setStyle(Style value)
```


يحصل أو يضبط نمط نطاقات الخلايا المُنسقة شرطياً.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| value | [Style](../../com.aspose.cells/style) |  |

### setText(String value) {#setText-java.lang.String-}
```
public void setText(String value)
```


القيمة النصية في قاعدة تنسيق شرطي "text contains". صالح فقط للنوع = containsText، notContainsText، beginsWith و endsWith. القيمة الافتراضية هي null.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | java.lang.String |  |

### setTimePeriod(int value) {#setTimePeriod-int-}
```
public void setTimePeriod(int value)
```


الفترة الزمنية المتاحة في قاعدة تنسيق شرطي "date occurrin". صالح فقط للنوع = timePeriod. القيمة الافتراضية هي TimePeriodType.Today.

انظر [TimePeriodType](../../com.aspose.cells/timeperiodtype).

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| القيمة | int |  |

### setType(int value) {#setType-int-}
```
public void setType(int value)
```


يضبط ما إذا كان نوع التنسيق الشرطي.

انظر [FormatConditionType](../../com.aspose.cells/formatconditiontype).

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

