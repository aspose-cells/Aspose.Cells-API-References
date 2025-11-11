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
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | Whether force given function to be recalculated always when calculating shared formulas. |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | Indicates whether this engine needs the parameter to be calculated in array mode. |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | Indicates whether this engine needs the literal text of parameter while doing calculation. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | Skips the calculation for the entire formula that references to the function currently under evaluation. |
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
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


Whether force given function to be recalculated always when calculating shared formulas.

**Remarks**

For shared formulas, multiple cells share the same function. If the function's parameters keep same for those cells too, then generally this function needs to be calculated only once. So for performance consideration we only calculate such kind of function once too([calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) is called only once, instead of being called repeatedly for every cell). However, for user's custom implementation, maybe the function, especially the custom function, needs to be calculated differently for different cells. If so, user needs to override this method to make it return true for the function. And for [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-), the given [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) may have been initialized with the cached value of previous calculation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionName | java.lang.String | name of the function. Generally it is custom function's name. If [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) is true, then built-in functions will also be checked here. |

**Returns:**
boolean - true if the specified function needs to be recalculated always.
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


Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. Default is false.

**Remarks**

If user needs to change the calculation logic of some built-in functions, this property should be set as true. Otherwise please leave this property as false for performance consideration.

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




### skipCalculation() {#skipCalculation--}
```
public void skipCalculation()
```


Skips the calculation for the entire formula that references to the function currently under evaluation.

**Remarks**

This method can be invoked in the implementation of [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) to skip the calculation for the entire formula and the original value of the formula will be kept without change.

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

