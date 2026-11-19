---
title: "GridAbstractCalculationEngine"
second_title: "Aspose.Cells for Java API Reference"
description: "يمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells."
type: docs
url: /ar/java/com.aspose.gridjs/gridabstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class GridAbstractCalculationEngine
```

يمثل محرك حساب مخصص للمستخدم لتوسيع محرك الحساب الافتراضي في Aspose.Cells.

**Remarks**

يجب على المستخدم عدم تعديل أي جزء من المصنف مباشرةً في هذا التنفيذ (باستثناء النتيجة المحسوبة للدالة المخصصة، والتي يمكن تعيينها عبر خاصية GridCalculationData.CalculatedValue property). وإلا قد يحدث نتيجة غير متوقعة أو Exception. إذا كان المستخدم بحاجة إلى تغيير بيانات أخرى غير النتيجة المحسوبة في التنفيذ لبعض الدوال المخصصة، على سبيل المثال، تغيير صيغة الخلية أو النمط... إلخ، يجب على المستخدم جمع تلك البيانات في هذا التنفيذ وتغييرها خارج نطاق حساب الصيغة.

**Example**

```
          class MyEngine extends GridAbstractCalculationEngine
         {
             public /*override*/ void calculate(GridCalculationData data)
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
                         if (pv instanceof GridReferredArea)
                         {
                             GridReferredArea ra = (GridReferredArea)pv;
                             pv = ra.getValue(0, 0);
                         }
                         //process the parameter here
                         //res = ...;
                     }
                     data.setCalculatedValue(res);
                 }
             }
         }
```
## المنشئات

| منشئ | الوصف |
| --- | --- |
| [GridAbstractCalculationEngine()](#GridAbstractCalculationEngine--) |  |
## الطرق

| طريقة | الوصف |
| --- | --- |
| [calculate(GridCalculationData data)](#calculate-com.aspose.gridjs.GridCalculationData-) | يحسب دالة واحدة باستخدام البيانات المعطاة. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridAbstractCalculationEngine() {#GridAbstractCalculationEngine--}
```
public GridAbstractCalculationEngine()
```


### calculate(GridCalculationData data) {#calculate-com.aspose.gridjs.GridCalculationData-}
```
public abstract void calculate(GridCalculationData data)
```


يحسب دالة واحدة باستخدام البيانات المعطاة.

**Remarks**

يجب على المستخدم تعيين القيمة المحسوبة للبيانات المعطاة لجميع الدوال (بما في ذلك الدوال الأصلية في Excel) التي يرغب في حسابها بنفسه في هذا التنفيذ.

**Parameters:**
| معامل | نوع | الوصف |
| --- | --- | --- |
| data | [GridCalculationData](../../com.aspose.gridjs/gridcalculationdata) | البيانات المطلوبة لحساب الدالة مثل اسم الدالة، المعلمات، ... إلخ. |

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
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

