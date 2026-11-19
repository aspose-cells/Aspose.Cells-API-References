---
title: "CalculationOptions"
second_title: "Aspose.Cells for Java API 参考"
description: "表示计算选项。"
type: docs
url: /zh/java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

表示计算选项。
## 构造函数

| 构造函数 | 描述 |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## 方法

| 方法 | 描述 |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | 递归计算单元格的堆栈大小。 |
| [getCalculationMonitor()](#getCalculationMonitor--) | 用于用户跟踪公式计算进度的监视器。 |
| [getCharacterEncoding()](#getCharacterEncoding--) | 指定在计算公式时用于字符编码/解码的编码方式。 |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | 自定义公式计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。 |
| [getIgnoreError()](#getIgnoreError--) | 指示在计算公式时是否应忽略遇到的错误。 |
| [getLinkedDataSources()](#getLinkedDataSources--) | 指定公式中使用的外部链接的数据源。 |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | 指定计算精度的处理策略。 |
| [getRecursive()](#getRecursive--) | 指示在计算一个单元格且该单元格依赖其他单元格时，是否递归计算其依赖单元格。 |
| [getRefreshDynamicArrayFormula()](#getRefreshDynamicArrayFormula--) | 指示是否在计算公式之前刷新动态数组公式。 |
| [getUserSpecifiedRefreshDynamicArrayFormula()](#getUserSpecifiedRefreshDynamicArrayFormula--) | 指示用户是否已明确指定在计算指定公式之前刷新动态数组公式的行为。 |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | 递归计算单元格的堆栈大小。 |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | 用于用户跟踪公式计算进度的监视器。 |
| [setCharacterEncoding(Encoding value)](#setCharacterEncoding-com.aspose.cells.Encoding-) | 指定在计算公式时用于字符编码/解码的编码方式。 |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | 自定义公式计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。 |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | 指示在计算公式时是否应忽略遇到的错误。 |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | 指定公式中使用的外部链接的数据源。 |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | 指定计算精度的处理策略。 |
| [setRecursive(boolean value)](#setRecursive-boolean-) | 指示在计算一个单元格且该单元格依赖其他单元格时，是否递归计算其依赖单元格。 |
| [setRefreshDynamicArrayFormula(boolean value)](#setRefreshDynamicArrayFormula-boolean-) | 指示是否在计算公式之前刷新动态数组公式。 |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CalculationOptions() {#CalculationOptions--}
```
public CalculationOptions()
```


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
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


递归计算单元格的堆栈大小。默认值为 200。

**Remarks**

当依赖树中需要递归计算的大量单元格时，计算过程中可能会导致 StackOverflowException。如果出现这种情况，用户应为此属性指定较小的值。对于此类情况，用户应根据实际公式和数据确定该属性的合适值。然而，值设得过小可能导致公式计算性能下降，且值小于 2 将使依赖其他公式的公式无法计算。因此，如果指定的值小于 2，将会被重置为 2。

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


用于用户跟踪公式计算进度的监视器。

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
### getCharacterEncoding() {#getCharacterEncoding--}
```
public Encoding getCharacterEncoding()
```


指定在计算公式时用于字符编码/解码的编码方式。对于 CHAR、CODE 等函数，计算结果取决于区域设置和环境的默认字符集。通过此属性，用户可以指定这些函数使用的适当编码，以获得预期的结果。

**Returns:**
[Encoding](../../com.aspose.cells/encoding)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCustomEngine() {#getCustomEngine--}
```
public AbstractCalculationEngine getCustomEngine()
```


自定义公式计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


指示在计算公式时是否应忽略遇到的错误。错误可能是不受支持的函数、外部链接等。默认值为 true。

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


指定公式中使用的外部链接的数据源。

**Remarks**

类似于 [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---)，在此您可以指定用于计算公式的外部链接的数据源，尤其是那些在 INDIRECT 函数中使用的外部链接。对于在 INDIRECT 函数中使用的外部链接，它们不会被视为工作簿的外部链接的一部分，且无法通过 [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) 更新。这些工作簿与外部链接的匹配由 [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) 和 [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) 决定。因此，请确保每个工作簿的 [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) 已使用适当的值（通常应与相应的 [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) 相同），以便它们能够按预期链接。

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


指定计算精度的处理策略。

参见 [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy)。

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


指示在计算一个单元格且该单元格依赖其他单元格时，是否递归计算其依赖单元格。默认值为 true。

**Returns:**
boolean
### getRefreshDynamicArrayFormula() {#getRefreshDynamicArrayFormula--}
```
public boolean getRefreshDynamicArrayFormula()
```


指示是否在计算公式之前刷新动态数组公式。

**Remarks**

If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), this property will be taken as true. For other cases, such as [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) or [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), this property will be taken as false.

**Returns:**
boolean
### getUserSpecifiedRefreshDynamicArrayFormula() {#getUserSpecifiedRefreshDynamicArrayFormula--}
```
public boolean getUserSpecifiedRefreshDynamicArrayFormula()
```


指示用户是否已明确指定在计算指定公式之前刷新动态数组公式的行为。

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




### setCalcStackSize(int value) {#setCalcStackSize-int-}
```
public void setCalcStackSize(int value)
```


递归计算单元格的堆栈大小。默认值为 200。

**Remarks**

当依赖树中需要递归计算的大量单元格时，计算过程中可能会导致 StackOverflowException。如果出现这种情况，用户应为此属性指定较小的值。对于此类情况，用户应根据实际公式和数据确定该属性的合适值。然而，值设得过小可能导致公式计算性能下降，且值小于 2 将使依赖其他公式的公式无法计算。因此，如果指定的值小于 2，将会被重置为 2。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


用于用户跟踪公式计算进度的监视器。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCharacterEncoding(Encoding value) {#setCharacterEncoding-com.aspose.cells.Encoding-}
```
public void setCharacterEncoding(Encoding value)
```


指定在计算公式时用于字符编码/解码的编码方式。对于 CHAR、CODE 等函数，计算结果取决于区域设置和环境的默认字符集。通过此属性，用户可以指定这些函数使用的适当编码，以获得预期的结果。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Encoding](../../com.aspose.cells/encoding) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


自定义公式计算引擎，用于扩展 Aspose.Cells 的默认计算引擎。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


指示在计算公式时是否应忽略遇到的错误。错误可能是不受支持的函数、外部链接等。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


指定公式中使用的外部链接的数据源。

**Remarks**

类似于 [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---)，在此您可以指定用于计算公式的外部链接的数据源，尤其是那些在 INDIRECT 函数中使用的外部链接。对于在 INDIRECT 函数中使用的外部链接，它们不会被视为工作簿的外部链接的一部分，且无法通过 [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---) 更新。这些工作簿与外部链接的匹配由 [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) 和 [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) 决定。因此，请确保每个工作簿的 [Workbook.getFileName()](../../com.aspose.cells/workbook\#getFileName--) 已使用适当的值（通常应与相应的 [ExternalLink.getDataSource()](../../com.aspose.cells/externallink\#getDataSource--) 相同），以便它们能够按预期链接。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


指定计算精度的处理策略。

参见 [CalculationPrecisionStrategy](../../com.aspose.cells/calculationprecisionstrategy)。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


指示在计算一个单元格且该单元格依赖其他单元格时，是否递归计算其依赖单元格。默认值为 true。

**Parameters:**
| 参数 | 类型 | 描述 |
| --- | --- | --- |
| 值 | boolean |  |

### setRefreshDynamicArrayFormula(boolean value) {#setRefreshDynamicArrayFormula-boolean-}
```
public void setRefreshDynamicArrayFormula(boolean value)
```


指示是否在计算公式之前刷新动态数组公式。

**Remarks**

If this property has been specified explicitly, then the specified value will be used to determine whether refresh dynamic array formulas. Otherwise([getUserSpecifiedRefreshDynamicArrayFormula()](../../com.aspose.cells/calculationoptions\#getUserSpecifiedRefreshDynamicArrayFormula--) is flase), the default value of it depends on what kind of formulas need to be calculated: For calculating formulas for the workbook, such as [Workbook.calculateFormula(CalculationOptions)](../../com.aspose.cells/workbook\#calculateFormula-CalculationOptions-), this property will be taken as true. For other cases, such as [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-) or [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), this property will be taken as false.

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

