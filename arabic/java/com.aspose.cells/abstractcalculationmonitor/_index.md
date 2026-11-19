---
title: "AbstractCalculationMonitor"
second_title: "Aspose.Cells for Java API Reference"
description: "مراقبة للمستخدم لتتبع تقدم حساب الصيغة."
type: docs
url: /ar/java/com.aspose.cells/abstractcalculationmonitor/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationMonitor
```

مراقبة للمستخدم لتتبع تقدم حساب الصيغة.

**Example**

```
         class MyCalculationMonitor extends AbstractCalculationMonitor
         {
             public /*override*/ void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
             {
                 if(sheetIndex!=0 || rowIndex!=0 || colIndex!=0)
                 {
                     return;
                 }
                 System.out.println("Cell A1 will be calculated.");
             }
         }
         Workbook wb = new Workbook("calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCalculationMonitor(new MyCalculationMonitor());
         wb.calculateFormula(opts);
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AbstractCalculationMonitor()](#AbstractCalculationMonitor--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [afterCalculate(int sheetIndex, int rowIndex, int colIndex)](#afterCalculate-int-int-int-) | نفّذ هذه الطريقة للقيام بالأعمال بعد حساب خلية واحدة. |
| [beforeCalculate(int sheetIndex, int rowIndex, int colIndex)](#beforeCalculate-int-int-int-) | نفّذ هذه الطريقة للقيام بالأعمال قبل حساب خلية واحدة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | يحصل على القيمة المحسوبة حديثًا للخلية. |
| [getClass()](#getClass--) |  |
| [getOriginalValue()](#getOriginalValue--) | يحصل على القيمة القديمة للخلية المحسوبة. |
| [getValueChanged()](#getValueChanged--) | ما إذا كانت قيمة الخلية قد تغيرت بعد الحساب. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [onCircular(Iterator circularCellsData)](#onCircular-java.util.Iterator-) | نفّذ هذه الطريقة للقيام بالأعمال عند حساب صيغ ذات مراجع دائرية. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationMonitor() {#AbstractCalculationMonitor--}
```
public AbstractCalculationMonitor()
```


### afterCalculate(int sheetIndex, int rowIndex, int colIndex) {#afterCalculate-int-int-int-}
```
public void afterCalculate(int sheetIndex, int rowIndex, int colIndex)
```


نفّذ هذه الطريقة للقيام بالأعمال بعد حساب خلية واحدة.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس الورقة التي تنتمي إليها الخلية. |
| rowIndex | int | فهرس الصف للخلية |
| colIndex | int | فهرس العمود للخلية |

### beforeCalculate(int sheetIndex, int rowIndex, int colIndex) {#beforeCalculate-int-int-int-}
```
public void beforeCalculate(int sheetIndex, int rowIndex, int colIndex)
```


نفّذ هذه الطريقة للقيام بالأعمال قبل حساب خلية واحدة.

**Remarks**

بالنسبة للخلايا في صيغ المصفوفة، قد لا يتم تنفيذ هذه الطريقة لأن هذه الخلايا عادةً تُحسب معًا.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| sheetIndex | int | فهرس الورقة التي تنتمي إليها الخلية. |
| rowIndex | int | فهرس الصف للخلية |
| colIndex | int | فهرس العمود للخلية |

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


يحصل على القيمة المحسوبة حديثًا للخلية. يجب استخدامها فقط في [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getOriginalValue() {#getOriginalValue--}
```
public Object getOriginalValue()
```


يحصل على القيمة القديمة للخلية المحسوبة. يجب استخدامها فقط في [beforeCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#beforeCalculate-int-int-int-) و [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
java.lang.Object
### getValueChanged() {#getValueChanged--}
```
public boolean getValueChanged()
```


ما إذا تم تغيير قيمة الخلية بعد الحساب. يجب استخدامها فقط في [afterCalculate(int,int,int)](../../com.aspose.cells/abstractcalculationmonitor\#afterCalculate-int-int-int-).

**Returns:**
boolean
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




### onCircular(Iterator circularCellsData) {#onCircular-java.util.Iterator-}
```
public boolean onCircular(Iterator circularCellsData)
```


نفّذ هذه الطريقة للقيام بالأعمال عند حساب صيغ ذات مراجع دائرية.

**Remarks**

في التنفيذ، قد يقوم المستخدم أيضًا بتعيين القيمة المتوقعة كنتيجة محسوبة لجزء/كل تلك الخلايا حتى لا يقوم محرك الصيغ بحسابها بشكل متكرر.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| circularCellsData | java.util.Iterator | IEnumerator مع عناصر [CalculationCell](../../com.aspose.cells/calculationcell) تمثل خلايا تعتمد على مراجع دائرية. |

**Returns:**
منطقي - ما إذا كان محرك الصيغ يحتاج إلى حساب تلك الخلايا بشكل دائري بعد هذه الاستدعاء. True للسماح لمحرك الصيغ بالاستمرار في حسابها. False للسماح لمحرك الصيغ فقط بوضع علامة على تلك الخلايا كـ Calculated.
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

