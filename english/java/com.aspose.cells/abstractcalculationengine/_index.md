---
title: AbstractCalculationEngine
second_title: Aspose.Cells for Java API Reference
description: Represents users custom calculation engine to extend the default calculation engine of Aspose.Cells.
type: docs
url: /java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.

**Remarks**

User should not modify any part of the Workbook directly in this implementation(except the calculated result of the custom function, which can be set by CalculationData.CalculatedValue property). Otherwise unexpected result or Exception may be caused. If user needs to change other data than calculated result in the implementation for some custom functions, for example, change cell's formula, style, ...etc., user should gather those data in this implementation and change them out of the scope of formula calculation.

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
## Constructors

| Constructor | Description |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## Methods

| Method | Description |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | Calculates one function with given data. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Indicates whether this engine needs the parameter to be calculated in array mode. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Indicates whether this engine needs the literal text of parameter while doing calculation. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
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


Calculates one function with given data.

**Remarks**

User should set the calculated value for given data for all functions(including excel native functions) that he wants to calculate by himself in this implementation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | the required data to calculate function such as function name, parameters, ...etc. |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| Parameter | Type | Description |
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
### getProcessBuiltInFunctions() {#getProcessBuiltInFunctions--}
```
public boolean getProcessBuiltInFunctions()
```


Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. Default is false. If user needs to change the calculation logic of some built-in functions, this property should be set as true. Otherwise please leave this property as false for performance consideration.

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


Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) is required when calculating custom functions and user has not updated the definition for them (by [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-)), this property needs to be set as true.

**Remarks**

If this custom calculation engine needs the parameter to be calculated in array mode, more stacks will be required to cache the tree for parameters and Calculate() method may be called recursively to calculate the parameter's value. For performance consideration, please keep this property as the default value(false) if there is no special requirement.

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false.

**Remarks**

If this custom calculation engine needs the parameter's literal text, more stacks will be required to cache the literal text for parameters and Calculate() method may be called recursively to calculate the parameter's value. Generally the literal text is not needed for calculating formulas and this property should be kept as false for most implementations to get better performance.

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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

