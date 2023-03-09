---
title: CalculationOptions
second_title: Aspose.Cells for Java API Reference
description: Represents options for calculation.
type: docs
url: /java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Represents options for calculation.
## Constructors

| Constructor | Description |
| --- | --- |
| [CalculationOptions()](#CalculationOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalcStackSize()](#getCalcStackSize--) | Specifies the stack size for calculating cells recursively. |
| [getCalculationMonitor()](#getCalculationMonitor--) | The monitor for user to track the progress of formula calculation. |
| [getClass()](#getClass--) |  |
| [getCustomEngine()](#getCustomEngine--) | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [getCustomFunction()](#getCustomFunction--) | The custom formula calculation functions to extend the calculation engine. |
| [getIgnoreError()](#getIgnoreError--) | Indicates if you need to hide the error in calculating formulas. |
| [getLinkedDataSources()](#getLinkedDataSources--) | Specifies the data sources for external links used in formulas. |
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Specifies the strategy for processing precision of calculation. |
| [getRecursive()](#getRecursive--) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | Specifies the stack size for calculating cells recursively. |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | The monitor for user to track the progress of formula calculation. |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | The custom formula calculation engine to extend the default calculation engine of Aspose.Cells. |
| [setCustomFunction(ICustomFunction value)](#setCustomFunction-com.aspose.cells.ICustomFunction-) | The custom formula calculation functions to extend the calculation engine. |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Indicates if you need to hide the error in calculating formulas. |
| [setLinkedDataSources(Workbook[] value)](#setLinkedDataSources-com.aspose.cells.Workbook---) | Specifies the data sources for external links used in formulas. |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Specifies the strategy for processing precision of calculation. |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. |
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
| Parameter | Type | Description |
| --- | --- | --- |
| arg0 | java.lang.Object |  |

**Returns:**
boolean
### getCalcStackSize() {#getCalcStackSize--}
```
public int getCalcStackSize()
```


Specifies the stack size for calculating cells recursively. When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. Too small value may cause performance degradation for the formula calculation.

**Returns:**
int
### getCalculationMonitor() {#getCalculationMonitor--}
```
public AbstractCalculationMonitor getCalculationMonitor()
```


The monitor for user to track the progress of formula calculation.

**Returns:**
[AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor)
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


The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.

**Returns:**
[AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine)
### getCustomFunction() {#getCustomFunction--}
```
public ICustomFunction getCustomFunction()
```


The custom formula calculation functions to extend the calculation engine. NOTE: This member is now obsolete. Instead, please use CustomEngine property, AbstractCalculationEngine provides more convenient and flexible APIs for manipulating custom functions. This property will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
[ICustomFunction](../../com.aspose.cells/icustomfunction)
### getIgnoreError() {#getIgnoreError--}
```
public boolean getIgnoreError()
```


Indicates if you need to hide the error in calculating formulas. The error may be unsupported function, external links, etc.

**Returns:**
boolean
### getLinkedDataSources() {#getLinkedDataSources--}
```
public Workbook[] getLinkedDataSources()
```


Specifies the data sources for external links used in formulas. Like [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---).

**Returns:**
com.aspose.cells.Workbook[]
### getPrecisionStrategy() {#getPrecisionStrategy--}
```
public int getPrecisionStrategy()
```


Specifies the strategy for processing precision of calculation.

**Returns:**
int
### getRecursive() {#getRecursive--}
```
public boolean getRecursive()
```


Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value if true.

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


Specifies the stack size for calculating cells recursively. When there are large amount of cells need to be calculated recursively in the dependency tree, StackOverflowException may be caused in the calculation process. If so, user should specify smaller value for this property. For such situation, user should determine the proper value for this property according to the actual formulas and data. Too small value may cause performance degradation for the formula calculation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


The monitor for user to track the progress of formula calculation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


The custom formula calculation engine to extend the default calculation engine of Aspose.Cells.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setCustomFunction(ICustomFunction value) {#setCustomFunction-com.aspose.cells.ICustomFunction-}
```
public void setCustomFunction(ICustomFunction value)
```


The custom formula calculation functions to extend the calculation engine. NOTE: This member is now obsolete. Instead, please use CustomEngine property, AbstractCalculationEngine provides more convenient and flexible APIs for manipulating custom functions. This property will be removed 12 months later since August 2020. Aspose apologizes for any inconvenience you may have experienced.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ICustomFunction](../../com.aspose.cells/icustomfunction) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Indicates if you need to hide the error in calculating formulas. The error may be unsupported function, external links, etc.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setLinkedDataSources(Workbook[] value) {#setLinkedDataSources-com.aspose.cells.Workbook---}
```
public void setLinkedDataSources(Workbook[] value)
```


Specifies the data sources for external links used in formulas. Like [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---), here you may specify data sources for external links used in formulas to be calculated, especially those used in INDIRECT function. For those external links used in INDIRECT function, they are not taken as part of the external links of the workbook and cannot be updated by [Workbook.updateLinkedDataSource(Workbook[])](../../com.aspose.cells/workbook\#updateLinkedDataSource-Workbook---).

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [Workbook\[\]](../../com.aspose.cells/workbook) |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Specifies the strategy for processing precision of calculation.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. The default value if true.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

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

