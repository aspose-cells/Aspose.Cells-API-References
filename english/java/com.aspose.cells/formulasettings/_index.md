---
title: FormulaSettings
second_title: Aspose.Cells for Java API Reference
description: Settings of formulas and calculation.
type: docs
weight: 238
url: /java/com.aspose.cells/formulasettings/
---

**Inheritance:**
java.lang.Object
```
public class FormulaSettings
```

Settings of formulas and calculation.
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculateOnOpen()](#getCalculateOnOpen--) | Indicates whether the application is required to perform a full calculation when the workbook is opened. |
| [getCalculateOnSave()](#getCalculateOnSave--) | Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. |
| [getCalculationId()](#getCalculationId--) | Specifies the version of the calculation engine used to calculate values in the workbook. |
| [getCalculationMode()](#getCalculationMode--) | the mode for workbook calculation in ms excel. |
| [getClass()](#getClass--) |  |
| [getEnableCalculationChain()](#getEnableCalculationChain--) | Whether enable calculation chain for formulas. |
| [getEnableIterativeCalculation()](#getEnableIterativeCalculation--) | Indicates whether enable iterative calculation to resolve circular references. |
| [getForceFullCalculation()](#getForceFullCalculation--) | Indicates whether calculates all formulas every time when a calculation is triggered. |
| [getMaxChange()](#getMaxChange--) | The maximum change to resolve a circular reference. |
| [getMaxIteration()](#getMaxIteration--) | The maximum iterations to resolve a circular reference. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | Whether the precision of calculated result be set as they are displayed while calculating formulas |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculateOnOpen(boolean value)](#setCalculateOnOpen-boolean-) | For the description of this property, please see [getCalculateOnOpen()](../../com.aspose.cells/formulasettings\#getCalculateOnOpen--) |
| [setCalculateOnSave(boolean value)](#setCalculateOnSave-boolean-) | For the description of this property, please see [getCalculateOnSave()](../../com.aspose.cells/formulasettings\#getCalculateOnSave--) |
| [setCalculationId(String value)](#setCalculationId-java.lang.String-) | For the description of this property, please see [getCalculationId()](../../com.aspose.cells/formulasettings\#getCalculationId--) |
| [setCalculationMode(int value)](#setCalculationMode-int-) | For the description of this property, please see [getCalculationMode()](../../com.aspose.cells/formulasettings\#getCalculationMode--) |
| [setEnableCalculationChain(boolean value)](#setEnableCalculationChain-boolean-) | For the description of this property, please see [getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--) |
| [setEnableIterativeCalculation(boolean value)](#setEnableIterativeCalculation-boolean-) | For the description of this property, please see [getEnableIterativeCalculation()](../../com.aspose.cells/formulasettings\#getEnableIterativeCalculation--) |
| [setForceFullCalculation(boolean value)](#setForceFullCalculation-boolean-) | For the description of this property, please see [getForceFullCalculation()](../../com.aspose.cells/formulasettings\#getForceFullCalculation--) |
| [setMaxChange(double value)](#setMaxChange-double-) | For the description of this property, please see [getMaxChange()](../../com.aspose.cells/formulasettings\#getMaxChange--) |
| [setMaxIteration(int value)](#setMaxIteration-int-) | For the description of this property, please see [getMaxIteration()](../../com.aspose.cells/formulasettings\#getMaxIteration--) |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | For the description of this property, please see [getPrecisionAsDisplayed()](../../com.aspose.cells/formulasettings\#getPrecisionAsDisplayed--) |
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
### getCalculateOnOpen() {#getCalculateOnOpen--}
```
public boolean getCalculateOnOpen()
```


Indicates whether the application is required to perform a full calculation when the workbook is opened. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

**Returns:**
boolean
### getCalculateOnSave() {#getCalculateOnSave--}
```
public boolean getCalculateOnSave()
```


Indicates whether recalculate the workbook before saving the document, when in manual calculation mode. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

**Returns:**
boolean
### getCalculationId() {#getCalculationId--}
```
public String getCalculationId()
```


Specifies the version of the calculation engine used to calculate values in the workbook. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. In the case of ms excel, if the value of this property is less than the recalculation engine identifier associated with the application that opens the resultant file, the application will recalculate the results of all formulas on this workbook immediately after loading the file. For performance consideration for most users' applications, we do not calculate any formula on the workbook automatically, no matter what value has been set for this property.

**Returns:**
java.lang.String
### getCalculationMode() {#getCalculationMode--}
```
public int getCalculationMode()
```


the mode for workbook calculation in ms excel. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most user's application, we do not calculate any formula in the workbook automatically, no matter what mode has been set for this property. If user needs to calculate formulas, please always call methods on different objects according to requirement: [Workbook.calculateFormula()](../../com.aspose.cells/workbook\#calculateFormula--), [Worksheet.calculateFormula(CalculationOptions,boolean)](../../com.aspose.cells/worksheet\#calculateFormula-CalculationOptions-boolean-), [Cell.calculate(CalculationOptions)](../../com.aspose.cells/cell\#calculate-CalculationOptions-), ...etc.

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


Whether enable calculation chain for formulas. Default is false. When there are lots of formulas in the workbook and user needs to calculate them repeatedly with modifying only a small part of them, it may be helpful for performance to enable the calculation chain. On the other hand, if the chain is enabled, maintaining the model of chain requires extra memory, and it also requires a bit more cpu time for some other operations such as changing cell's value or formulas. After changing this property from false to true, the calculation chain will be analyzed and built at the time of first calculation for the workbook, so the required time for the first calculation may be more than normal calculation without chain.

**Returns:**
boolean
### getEnableIterativeCalculation() {#getEnableIterativeCalculation--}
```
public boolean getEnableIterativeCalculation()
```


Indicates whether enable iterative calculation to resolve circular references.

**Returns:**
boolean
### getForceFullCalculation() {#getForceFullCalculation--}
```
public boolean getForceFullCalculation()
```


Indicates whether calculates all formulas every time when a calculation is triggered. This property is only for saving the settings to resultant spreadsheet file so that other applications(such as ms excel) may act accordingly when loading and manipulating the resultant file. For performance consideration for most users' applications, we do not calculate any formula in the workbook automatically, no matter what value has been set for this property.

**Returns:**
boolean
### getMaxChange() {#getMaxChange--}
```
public double getMaxChange()
```


The maximum change to resolve a circular reference.

**Returns:**
double
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


The maximum iterations to resolve a circular reference.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


Whether the precision of calculated result be set as they are displayed while calculating formulas

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


For the description of this property, please see [getCalculateOnOpen()](../../com.aspose.cells/formulasettings\#getCalculateOnOpen--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCalculateOnSave(boolean value) {#setCalculateOnSave-boolean-}
```
public void setCalculateOnSave(boolean value)
```


For the description of this property, please see [getCalculateOnSave()](../../com.aspose.cells/formulasettings\#getCalculateOnSave--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCalculationId(String value) {#setCalculationId-java.lang.String-}
```
public void setCalculationId(String value)
```


For the description of this property, please see [getCalculationId()](../../com.aspose.cells/formulasettings\#getCalculationId--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCalculationMode(int value) {#setCalculationMode-int-}
```
public void setCalculationMode(int value)
```


For the description of this property, please see [getCalculationMode()](../../com.aspose.cells/formulasettings\#getCalculationMode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setEnableCalculationChain(boolean value) {#setEnableCalculationChain-boolean-}
```
public void setEnableCalculationChain(boolean value)
```


For the description of this property, please see [getEnableCalculationChain()](../../com.aspose.cells/formulasettings\#getEnableCalculationChain--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableIterativeCalculation(boolean value) {#setEnableIterativeCalculation-boolean-}
```
public void setEnableIterativeCalculation(boolean value)
```


For the description of this property, please see [getEnableIterativeCalculation()](../../com.aspose.cells/formulasettings\#getEnableIterativeCalculation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setForceFullCalculation(boolean value) {#setForceFullCalculation-boolean-}
```
public void setForceFullCalculation(boolean value)
```


For the description of this property, please see [getForceFullCalculation()](../../com.aspose.cells/formulasettings\#getForceFullCalculation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMaxChange(double value) {#setMaxChange-double-}
```
public void setMaxChange(double value)
```


For the description of this property, please see [getMaxChange()](../../com.aspose.cells/formulasettings\#getMaxChange--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


For the description of this property, please see [getMaxIteration()](../../com.aspose.cells/formulasettings\#getMaxIteration--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


For the description of this property, please see [getPrecisionAsDisplayed()](../../com.aspose.cells/formulasettings\#getPrecisionAsDisplayed--)

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

