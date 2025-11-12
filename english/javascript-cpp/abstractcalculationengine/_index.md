---
title: AbstractCalculationEngine
second_title: Aspose.Cells for JavaScript via C++ API Reference
description: Represents users custom calculation engine to extend the default calculation engine of Aspose.Cells.
type: docs
url: /javascript-cpp/abstractcalculationengine/
---

## AbstractCalculationEngine class

Represents user's custom calculation engine to extend the default calculation engine of Aspose.Cells.

```javascript
abstract class AbstractCalculationEngine;
```

### Remarks
User should not modify any part of the Workbook directly in this implementation(except the calculated result of the custom function, which can be set by CalculationData.CalculatedValue property). Otherwise unexpected result or Exception may be caused. If user needs to change other data than calculated result in the implementation for some custom functions, for example, change cell's formula, style, ...etc., user should gather those data in this implementation and change them out of the scope of formula calculation.

## Methods

| Method | Description |
| --- | --- |
| [skipCalculation()](#skipCalculation--)| Skips the calculation for the entire formula that references to the function currently under evaluation. |
| abstract [isParamLiteralRequired()](#isParamLiteralRequired--)| Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false. |
| abstract [isParamArrayModeRequired()](#isParamArrayModeRequired--)| Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If [CalculationData.GetParamValueInArrayMode(int, int, int)](../calculationdata.getparamvalueinarraymode(int, int, int)/) is required when calculating custom functions and user has not updated the definition for them (by [Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)](../workbook.updatecustomfunctiondefinition(customfunctiondefinition)/)), this property needs to be set as true. |
| abstract [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--)| Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. Default is false. |
| abstract [calculate(CalculationData)](#calculate-calculationdata-)| Calculates one function with given data. |
| abstract [forceRecalculate(string)](#forceRecalculate-string-)| Whether force given function to be recalculated always when calculating shared formulas. |


### skipCalculation() {#skipCalculation--}

Skips the calculation for the entire formula that references to the function currently under evaluation.

```javascript
skipCalculation() : void;
```


**Remarks**

This method can be invoked in the implementation of [Calculate(CalculationData)](../calculate(calculationdata)/) to skip the calculation for the entire formula and the original value of the formula will be kept without change.

### isParamLiteralRequired() {#isParamLiteralRequired--}

Indicates whether this engine needs the literal text of parameter while doing calculation. Default value is false.

```javascript
abstract isParamLiteralRequired() : boolean;
```


**Remarks**

If this custom calculation engine needs the parameter's literal text, more stacks will be required to cache the literal text for parameters and Calculate() method may be called recursively to calculate the parameter's value. Generally the literal text is not needed for calculating formulas and this property should be kept as false for most implementations to get better performance.

### isParamArrayModeRequired() {#isParamArrayModeRequired--}

Indicates whether this engine needs the parameter to be calculated in array mode. Default value is false. If [CalculationData.GetParamValueInArrayMode(int, int, int)](../calculationdata.getparamvalueinarraymode(int, int, int)/) is required when calculating custom functions and user has not updated the definition for them (by [Workbook.UpdateCustomFunctionDefinition(CustomFunctionDefinition)](../workbook.updatecustomfunctiondefinition(customfunctiondefinition)/)), this property needs to be set as true.

```javascript
abstract isParamArrayModeRequired() : boolean;
```


**Remarks**

If this custom calculation engine needs the parameter to be calculated in array mode, more stacks will be required to cache the tree for parameters and Calculate() method may be called recursively to calculate the parameter's value. For performance consideration, please keep this property as the default value(false) if there is no special requirement.

### getProcessBuiltInFunctions() {#getProcessBuiltInFunctions--}

Whether built-in functions that have been supported by the built-in engine should be checked and processed by this implementation. Default is false.

```javascript
abstract getProcessBuiltInFunctions() : boolean;
```


**Remarks**

If user needs to change the calculation logic of some built-in functions, this property should be set as true. Otherwise please leave this property as false for performance consideration.

### calculate(CalculationData) {#calculate-calculationdata-}

Calculates one function with given data.

```javascript
abstract calculate(data: CalculationData) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| data | [CalculationData](../calculationdata/) | the required data to calculate function such as function name, parameters, ...etc. |

**Remarks**

User should set the calculated value for given data for all functions(including excel native functions) that he wants to calculate by himself in this implementation.

### forceRecalculate(string) {#forceRecalculate-string-}

Whether force given function to be recalculated always when calculating shared formulas.

```javascript
abstract forceRecalculate(functionName: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| functionName | string | name of the function. Generally it is custom function's name.         /// If [ProcessBuiltInFunctions](../processbuiltinfunctions/) is true, then built-in functions will also be checked here. |

**Returns**

true if the specified function needs to be recalculated always.

**Remarks**

For shared formulas, multiple cells share the same function. If the function's parameters keep same for those cells too, then generally this function needs to be calculated only once. So for performance consideration we only calculate such kind of function once too([Calculate(CalculationData)](../calculate(calculationdata)/) is called only once, instead of being called repeatedly for every cell). However, for user's custom implementation, maybe the function, especially the custom function, needs to be calculated differently for different cells. If so, user needs to override this method to make it return true for the function. And for [Calculate(CalculationData)](../calculate(calculationdata)/), the given [CalculationData.CalculatedValue](../calculationdata.calculatedvalue/) may have been initialized with the cached value of previous calculation.


