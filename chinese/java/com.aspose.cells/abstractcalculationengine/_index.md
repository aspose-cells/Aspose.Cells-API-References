---
title: "AbstractCalculationEngine"
second_title: "Aspose.Cells for Java API 参考"
description: "表示用户的自定义计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。"
type: docs
url: /zh/java/com.aspose.cells/abstractcalculationengine/
---

**Inheritance:**
java.lang.Object
```
public abstract class AbstractCalculationEngine
```

表示用户的自定义计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。

**Remarks**

用户不应在此实现中直接修改 Workbook 的任何部分（除非是自定义函数的计算结果，该结果可通过 CalculationData.CalculatedValue 属性设置）。否则可能导致意外结果或异常。如果用户需要在实现中更改除计算结果之外的其他数据，例如更改单元格的公式、样式等，用户应在此实现中收集这些数据并在公式计算范围之外进行更改。

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
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [AbstractCalculationEngine()](#AbstractCalculationEngine--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [calculate(CalculationData data)](#calculate-com.aspose.cells.CalculationData-) | 使用给定数据计算一个函数。 |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [forceRecalculate(String functionName)](#forceRecalculate-java.lang.String-) | 在计算共享公式时，是否强制始终重新计算给定函数。 |
| [getClass()](#getClass--) |  |
| [getProcessBuiltInFunctions()](#getProcessBuiltInFunctions--) | 是否应检查并由此实现处理已被内置引擎支持的内置函数。 |
| [hashCode()](#hashCode--) |  |
| [isParamArrayModeRequired()](#isParamArrayModeRequired--) | 指示此引擎是否需要以数组模式计算参数。 |
| [isParamLiteralRequired()](#isParamLiteralRequired--) | 指示此引擎在计算时是否需要参数的文字文本。 |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [skipCalculation()](#skipCalculation--) | 跳过对引用当前正在评估的函数的整个公式的计算。 |
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


使用给定数据计算一个函数。

**Remarks**

用户应为给定数据设置所有函数（包括 Excel 原生函数）的计算值，以便在此实现中自行计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| data | [CalculationData](../../com.aspose.cells/calculationdata) | 计算函数所需的数据，例如函数名称、参数等。 |

### equals(Object arg0) {#equals-java.lang.Object-}
```
public boolean equals(Object arg0)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### forceRecalculate(String functionName) {#forceRecalculate-java.lang.String-}
```
public boolean forceRecalculate(String functionName)
```


在计算共享公式时，是否强制始终重新计算给定函数。

**Remarks**

对于共享公式，多个单元格共享同一个函数。如果这些单元格的函数参数也保持相同，则通常该函数只需计算一次。因此出于性能考虑，我们也只会计算此类函数一次（[calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) 只调用一次，而不是对每个单元格重复调用）。然而，对于用户的自定义实现，函数（尤其是自定义函数）可能需要针对不同单元格进行不同的计算。如果是这种情况，用户需要重写此方法，使其对该函数返回 true。并且对于 [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-)，给定的 [CalculationData.getCalculatedValue()](../../com.aspose.cells/calculationdata\#getCalculatedValue--) 可能已经使用上一次计算的缓存值进行初始化。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| functionName | java.lang.String | 函数的名称。通常是自定义函数的名称。如果 [getProcessBuiltInFunctions()](../../com.aspose.cells/abstractcalculationengine\#getProcessBuiltInFunctions--) 为 true，则也会检查内置函数。 |

**Returns:**
布尔值 - 如果指定函数需要始终重新计算则为 true。
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


是否应检查并由此实现处理已被内置引擎支持的内置函数。默认值为 false。

**Remarks**

如果用户需要更改某些内置函数的计算逻辑，应将此属性设为 true。否则请保持此属性为 false，以考虑性能。

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


指示此引擎是否需要以数组模式计算参数。默认值为 false。如果在计算自定义函数时需要使用 [CalculationData.getParamValueInArrayMode(int,int,int)](../../com.aspose.cells/calculationdata\#getParamValueInArrayMode-int-int-int-) 且用户尚未通过 [Workbook.updateCustomFunctionDefinition(CustomFunctionDefinition)](../../com.aspose.cells/workbook\#updateCustomFunctionDefinition-CustomFunctionDefinition-) 更新其定义，则需要将此属性设为 true。

**Remarks**

如果此自定义计算引擎需要以数组模式计算参数，则需要更多的栈来缓存参数的树结构，Calculate() 方法可能会递归调用以计算参数的值。出于性能考虑，如果没有特殊需求，请保持此属性的默认值（false）。

**Returns:**
boolean
### isParamLiteralRequired() {#isParamLiteralRequired--}
```
public boolean isParamLiteralRequired()
```


指示此引擎在计算时是否需要参数的文字文本。默认值为 false。

**Remarks**

如果此自定义计算引擎需要参数的文字文本，则需要更多的栈来缓存参数的文字文本，Calculate() 方法可能会递归调用以计算参数的值。通常在计算公式时不需要文字文本，为了获得更好的性能，大多数实现应将此属性保持为 false。

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


跳过对引用当前正在评估的函数的整个公式的计算。

**Remarks**

此方法可在 [calculate(CalculationData)](../../com.aspose.cells/abstractcalculationengine\#calculate-CalculationData-) 的实现中调用，以跳过对整个公式的计算，公式的原始值将保持不变。

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
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |

### wait(long arg0, int arg1) {#wait-long-int-}
```
public final void wait(long arg0, int arg1)
```




**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| arg0 | long |  |
| arg1 | int |  |

