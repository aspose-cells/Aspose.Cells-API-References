---
title: "AbstractCalculationEngine"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells."
type: docs
url: /ar/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

يمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

**Remarks**

يجب على المستخدم عدم تعديل أي جزء من المصنف (Workbook) مباشرةً في هذا التنفيذ (باستثناء النتيجة المحسوبة للدالة المخصصة، والتي يمكن تعيينها عبر الخاصية CalculationData.CalculatedValue). وإلا قد يحدث نتيجة غير متوقعة أو استثناء. إذا كان المستخدم بحاجة إلى تغيير بيانات أخرى غير النتيجة المحسوبة في التنفيذ لبعض الدوال المخصصة، على سبيل المثال، تغيير صيغة الخلية أو نمطها، ...إلخ، يجب على المستخدم جمع تلك البيانات في هذا التنفيذ وتغييرها خارج نطاق حساب الصيغة.

**Example**

```
         class MyEngine extends AbstractCalculationEngine
         {
             public /*override*/ void calculate(CalculationData data)
             {
                 String funcName = data.getFunctionName().toUpperCase();
                 if ("MYFUNC".equals(funcName))
                 {
                     //do calculation for MYFUNC here
                     int count = data.getParamCount();
                     Object res = null;
                     for (int i = 0; i <count; i++)
                     {
                         Object pv = data.getParamValue(i);
                         if (pv instanceof ReferredArea)
                         {
                             ReferredArea ra = (ReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
         Workbook wb = new Workbook("custom_calc.xlsx");
         CalculationOptions opts = new CalculationOptions();
         opts.setCustomEngine(new MyEngine());
         wb.calculateFormula(opts);
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | يحسب دالة واحدة باستخدام البيانات المعطاة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | ما إذا كان يجب إجبار الدالة المعطاة على إعادة حسابها دائمًا عند حساب الصيغ المشتركة. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | ما إذا كان يجب فحص ومعالجة الدوال المدمجة التي يدعمها المحرك المدمج بواسطة هذا التنفيذ. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | يشير إلى ما إذا كان هذا المحرك يحتاج إلى حساب المعامل في وضع المصفوفة. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | يشير إلى ما إذا كان هذا المحرك يحتاج إلى النص الحرفي للمعامل أثناء إجراء الحساب. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | يتخطى حساب الصيغة بالكامل التي تشير إلى الدالة التي يتم تقييمها حاليًا. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AbstractCalculationEngine() {#AbstractCalculationEngine--}
```
public AbstractCalculationEngine()
```


### calculate(CalculationData data) {#calculate-com.aspose.cells.CalculationData-}
```
public abstract void calculate(CalculationData data)
```


يحسب دالة واحدة باستخدام البيانات المعطاة.

**Remarks**

يجب على المستخدم تعيين القيمة المحسوبة للبيانات المعطاة لجميع الدوال (بما في ذلك الدوال الأصلية في Excel) التي يرغب في حسابها بنفسه في هذا التنفيذ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | البيانات المطلوبة لحساب الدالة مثل اسم الدالة، المعاملات، ...إلخ. |

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
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


ما إذا كان يجب إجبار الدالة المعطاة على إعادة حسابها دائمًا عند حساب الصيغ المشتركة.

**Remarks**

بالنسبة للصيغ المشتركة، تشترك عدة خلايا في نفس الدالة. إذا كانت معاملات الدالة تبقى نفسها لتلك الخلايا أيضًا، فإن هذه الدالة عادةً تحتاج إلى حسابها مرة واحدة فقط. لذا، من منظور الأداء، نحسب هذا النوع من الدوال مرة واحدة فقط أيضًا ([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) يُستدعى مرة واحدة فقط، بدلاً من استدعائه بشكل متكرر لكل خلية). ومع ذلك، في تنفيذ المستخدم المخصص، قد تحتاج الدالة، خاصة الدالة المخصصة، إلى حساب مختلف للخلايا المختلفة. إذا كان الأمر كذلك، يجب على المستخدم تجاوز هذه الطريقة لجعلها تُعيد true لهذه الدالة. وبالنسبة إلى [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-)، قد تكون القيمة المعطاة من [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) قد تم تهيئتها بالقيمة المخزنة من الحساب السابق.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| functionName | java.lang.String | اسم الدالة. عادةً ما يكون اسم الدالة المخصصة. إذا كان [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) true، فسيتم فحص الدوال المدمجة هنا أيضًا. |

**Returns:**
منطقي - true إذا كانت الدالة المحددة تحتاج إلى إعادة حسابها دائمًا.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getProcessBuiltInFunctions() {#getProcessBuiltInFunctions--}
```
public boolean getProcessBuiltInFunctions()
```


ما إذا كان يجب فحص ومعالجة الدوال المدمجة التي يدعمها المحرك المدمج بواسطة هذا التنفيذ. القيمة الافتراضية هي false.

**Remarks**

إذا كان المستخدم بحاجة إلى تغيير منطق حساب بعض الدوال المدمجة، يجب تعيين هذه الخاصية إلى true. وإلا يرجى ترك هذه الخاصية على false لأسباب تتعلق بالأداء.

**Returns:**
boolean
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isParamArrayModeRequired() {#isParamArrayModeRequired--}
```
public boolean isParamArrayModeRequired()
```


يشير إلى ما إذا كان هذا المحرك يحتاج إلى حساب المعامل في وضع المصفوفة. القيمة الافتراضية هي false. إذا كان [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) مطلوبًا عند حساب الدوال المخصصة ولم يقم المستخدم بتحديث التعريف لها (عن طريق [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-))، يجب تعيين هذه الخاصية إلى true.

**Remarks**

إذا كان محرك الحساب المخصص هذا يحتاج إلى حساب المعامل في وضع المصفوفة، فستحتاج إلى مزيد من المكدسات لتخزين شجرة المعاملات وقد يتم استدعاء طريقة Calculate() بشكل متكرر لحساب قيمة المعامل. من منظور الأداء، يرجى ترك هذه الخاصية على القيمة الافتراضية (false) إذا لم يكن هناك أي متطلبات خاصة.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


يشير إلى ما إذا كان هذا المحرك يحتاج إلى النص الحرفي للمعامل أثناء إجراء حساب. القيمة الافتراضية هي false.

**Remarks**

إذا كان محرك الحساب المخصص هذا يحتاج إلى النص الحرفي للمعامل، سيتطلب المزيد من المكدسات لتخزين النص الحرفي للمعاملات وقد يتم استدعاء طريقة Calculate() بشكل متكرر لحساب قيمة المعامل. بشكل عام، لا يكون النص الحرفي مطلوبًا لحساب الصيغ ويجب إبقاء هذه الخاصية على false لمعظم التطبيقات للحصول على أداء أفضل.

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




### skipCalculation() {#skipCalculation--}
```
public void skipCalculation()
```


يتخطى حساب الصيغة بالكامل التي تشير إلى الدالة التي يتم تقييمها حاليًا.

**Remarks**

يمكن استدعاء هذه الطريقة في تنفيذ [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) لتخطي الحساب للمعادلة بأكملها وسيتم الحفاظ على القيمة الأصلية للمعادلة دون تغيير.

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

