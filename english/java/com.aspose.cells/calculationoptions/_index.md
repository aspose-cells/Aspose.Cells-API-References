---
title: CalculationOptions
second_title: Aspose.Cells for Java API Reference
description: Represents options for calculation.
type: docs
weight: 53
url: /java/com.aspose.cells/calculationoptions/
---

**Inheritance:**
java.lang.Object
```
public class CalculationOptions
```

Represents options for calculation.
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
| [getPrecisionStrategy()](#getPrecisionStrategy--) | Specifies the strategy for processing precision of calculation. |
| [getRecursive()](#getRecursive--) | Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalcStackSize(int value)](#setCalcStackSize-int-) | Please see the getter of this property: @CREF723\_ |
| [setCalculationMonitor(AbstractCalculationMonitor value)](#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-) | Please see the getter of this property: @CREF722\_ |
| [setCustomEngine(AbstractCalculationEngine value)](#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-) | Please see the getter of this property: @CREF721\_ |
| [setCustomFunction(ICustomFunction value)](#setCustomFunction-com.aspose.cells.ICustomFunction-) | Please see the getter of this property: @CREF720\_ |
| [setIgnoreError(boolean value)](#setIgnoreError-boolean-) | Please see the getter of this property: @CREF719\_ |
| [setPrecisionStrategy(int value)](#setPrecisionStrategy-int-) | Please see the getter of this property: @CREF724\_ |
| [setRecursive(boolean value)](#setRecursive-boolean-) | Please see the getter of this property: @CREF725\_ |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
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


Indicates whether calculate the dependent cells recursively when calculating one cell and it depends on other cells.

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


Please see the getter of this property: @CREF723\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setCalculationMonitor(AbstractCalculationMonitor value) {#setCalculationMonitor-com.aspose.cells.AbstractCalculationMonitor-}
```
public void setCalculationMonitor(AbstractCalculationMonitor value)
```


Please see the getter of this property: @CREF722\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationMonitor](../../com.aspose.cells/abstractcalculationmonitor) |  |

### setCustomEngine(AbstractCalculationEngine value) {#setCustomEngine-com.aspose.cells.AbstractCalculationEngine-}
```
public void setCustomEngine(AbstractCalculationEngine value)
```


Please see the getter of this property: @CREF721\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractCalculationEngine](../../com.aspose.cells/abstractcalculationengine) |  |

### setCustomFunction(ICustomFunction value) {#setCustomFunction-com.aspose.cells.ICustomFunction-}
```
public void setCustomFunction(ICustomFunction value)
```


Please see the getter of this property: @CREF720\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [ICustomFunction](../../com.aspose.cells/icustomfunction) |  |

### setIgnoreError(boolean value) {#setIgnoreError-boolean-}
```
public void setIgnoreError(boolean value)
```


Please see the getter of this property: @CREF719\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setPrecisionStrategy(int value) {#setPrecisionStrategy-int-}
```
public void setPrecisionStrategy(int value)
```


Please see the getter of this property: @CREF724\_

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRecursive(boolean value) {#setRecursive-boolean-}
```
public void setRecursive(boolean value)
```


Please see the getter of this property: @CREF725\_

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

