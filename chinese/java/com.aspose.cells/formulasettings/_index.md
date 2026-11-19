---
title: "FormulaSettings"
second_title: "Aspose.Cells for Java API 参考"
description: "公式和计算的设置。"
type: docs
url: /zh/java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

公式和计算的设置。
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | 指示在打开工作簿时，应用程序是否需要执行完整计算。 |
| [getCalculateOnSave()](#getCalculateOnSave--) | 指示在手动计算模式下，是否在保存文档前重新计算工作簿。 |
| [getCalculationId()](#getCalculationId--) | 指定用于计算工作簿中数值的计算引擎版本。 |
| [getCalculationMode()](#getCalculationMode--) | 获取在 MS Excel 中的工作簿计算模式。 |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | 指示是否为公式启用计算链。 |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | 指示是否启用迭代计算以解决循环引用。 |
| [getForceFullCalculation()](#getForceFullCalculation--) | 指示在触发计算时是否每次都计算所有公式。 |
| [getMaxChange()](#getMaxChange--) | 解决循环引用的最大变化量。 |
| [getMaxIteration()](#getMaxIteration--) | 解决循环引用的最大迭代次数。 |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | 指示在计算公式时，计算结果的精度是否设置为显示的方式。 |
| [getPreservePaddingSpaces()](#getPreservePaddingSpaces--) | 指示在获取和设置公式时，是否保留公式标记之间填充的空格和换行符。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | 指示在打开工作簿时，应用程序是否需要执行完整计算。 |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | 指示在手动计算模式下，是否在保存文档前重新计算工作簿。 |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | 指定用于计算工作簿中数值的计算引擎版本。 |
| [setCalculationMode(int value)](#setCalculationMode-int-) | 设置在 MS Excel 中的工作簿计算模式。 |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | 指示是否为公式启用计算链。 |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | 指示是否启用迭代计算以解决循环引用。 |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | 指示在触发计算时是否每次都计算所有公式。 |
| [setMaxChange(double value)](#setMaxChange-double-) | 解决循环引用的最大变化量。 |
| [setMaxIteration(int value)](#setMaxIteration-int-) | 解决循环引用的最大迭代次数。 |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | 指示在计算公式时，计算结果的精度是否设置为显示的方式。 |
| [setPreservePaddingSpaces(boolean value)](#setPreservePaddingSpaces-boolean-) | 指示在获取和设置公式时，是否保留公式标记之间填充的空格和换行符。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


指示在打开工作簿时，应用程序是否需要执行完整计算。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载生成的文件时能够相应地处理。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何值。

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


指示在手动计算模式下，是否在保存文档前重新计算工作簿。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载和操作生成的文件时能够相应地处理。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何值。

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


指定用于计算工作簿中数值的计算引擎版本。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载和操作生成的文件时能够相应地处理。对于 ms excel，如果此属性的值小于打开生成文件的应用程序关联的重新计算引擎标识符，应用程序将在加载文件后立即重新计算工作簿中所有公式的结果。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何值。

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


获取在 MS Excel 中的工作簿计算模式。

参见 [CalcModeType](../../com.aspose.cells/calcmodetype)。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载和操作生成的文件时能够相应地处理。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何模式。如果用户需要计算公式，请始终根据需求调用不同对象上的方法：[Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--)、[Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-)、[Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-)、...等。

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getEnableCalculationChain() {#getEnableCalculationChain--}
```
public boolean getEnableCalculationChain()
```


指示是否为公式启用计算链。默认值为 false。

**Remarks**

当工作簿中有大量公式且用户仅修改其中一小部分后需要重复计算时，启用计算链可能有助于提升性能。另一方面，如果启用链，维护链模型会占用额外内存，并且在更改单元格的值或公式等其他操作时会消耗更多 CPU 时间。将此属性从 false 改为 true 后，计算链将在工作簿的首次计算时进行分析并构建，因此首次计算所需的时间可能会超过未使用链的普通计算。

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


指示是否启用迭代计算以解决循环引用。

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


指示在触发计算时是否每次都计算所有公式。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载和操作生成的文件时能够相应地处理。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何值。

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


解决循环引用的最大变化量。

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


解决循环引用的最大迭代次数。

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


指示在计算公式时，计算结果的精度是否设置为显示的方式。

**Returns:**
boolean
### getPreservePaddingSpaces() {#getPreservePaddingSpaces--}
```
public boolean getPreservePaddingSpaces()
```


指示在获取和设置公式时，是否保留公式标记之间填充的空格和换行符。默认值为 false。

**Remarks**

通常这些空格和换行符仅用于视觉效果，是否保留它们并不影响计算结果。出于性能考虑，如果没有特殊需求，处理公式时最好不要保留它们。

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




### setCalculateOnOpen(boolean value) {#setCalculateOnOpen-boolean-}
```
public void setCalculateOnOpen(boolean value)
```


指示在打开工作簿时，应用程序是否需要执行完整计算。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载生成的文件时能够相应地处理。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


指示在手动计算模式下，是否在保存文档前重新计算工作簿。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载和操作生成的文件时能够相应地处理。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


指定用于计算工作簿中数值的计算引擎版本。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载和操作生成的文件时能够相应地处理。对于 ms excel，如果此属性的值小于打开生成文件的应用程序关联的重新计算引擎标识符，应用程序将在加载文件后立即重新计算工作簿中所有公式的结果。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


设置在 MS Excel 中的工作簿计算模式。

参见 [CalcModeType](../../com.aspose.cells/calcmodetype)。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载和操作生成的文件时能够相应地处理。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何模式。如果用户需要计算公式，请始终根据需求调用不同对象上的方法：[Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--)、[Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-)、[Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-)、...等。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


指示是否为公式启用计算链。默认值为 false。

**Remarks**

当工作簿中有大量公式且用户仅修改其中一小部分后需要重复计算时，启用计算链可能有助于提升性能。另一方面，如果启用链，维护链模型会占用额外内存，并且在更改单元格的值或公式等其他操作时会消耗更多 CPU 时间。将此属性从 false 改为 true 后，计算链将在工作簿的首次计算时进行分析并构建，因此首次计算所需的时间可能会超过未使用链的普通计算。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


指示是否启用迭代计算以解决循环引用。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


指示在触发计算时是否每次都计算所有公式。

**Remarks**

此属性仅用于将设置保存到生成的电子表格文件，以便其他应用程序（例如 ms excel）在加载和操作生成的文件时能够相应地处理。出于对大多数用户应用程序的性能考虑，我们不会自动计算工作簿中的任何公式，无论此属性设置为何值。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


解决循环引用的最大变化量。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


解决循环引用的最大迭代次数。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


指示在计算公式时，计算结果的精度是否设置为显示的方式。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setPreservePaddingSpaces(boolean value) {#setPreservePaddingSpaces-boolean-}
```
public void setPreservePaddingSpaces(boolean value)
```


指示在获取和设置公式时，是否保留公式标记之间填充的空格和换行符。默认值为 false。

**Remarks**

通常这些空格和换行符仅用于视觉效果，是否保留它们并不影响计算结果。出于性能考虑，如果没有特殊需求，处理公式时最好不要保留它们。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

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

