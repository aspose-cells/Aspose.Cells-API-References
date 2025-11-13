---
title: GridWorkbookSettings
second_title: Aspose.Cells for Java API Reference
description: Represents the settings of the workbook.
type: docs
url: /java/com.aspose.gridjs/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Represents the settings of the workbook.

**Example**

```
         GridJsWorkbook g = new GridJsWorkbook();
 
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         g.setSettings(gsettings);
 
         //do your business
```
## Constructors

| Constructor | Description |
| --- | --- |
| [GridWorkbookSettings()](#GridWorkbookSettings--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAuthor()](#getAuthor--) | Gets the author of the file. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | Indicates whether checking custom number format when setting Style.Custom, default is false. |
| [getCheckExcelRestriction()](#getCheckExcelRestriction--) | Whether check restriction of excel file when user modify cells related objects. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | Indicates whether create calculated formulas chain. |
| [getDate1904()](#getDate1904--) | Gets a value which represents if the workbook uses the 1904 date system. |
| [getEnableMacros()](#getEnableMacros--) | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [getForceFullCalculate()](#getForceFullCalculate--) | Indicates whether fully calculates every time when a calculation is triggered. |
| [getIteration()](#getIteration--) | Indicates whether use iteration to resolve circular references. |
| [getMaxIteration()](#getMaxIteration--) | Returns or sets the maximum number of iterations to resolve a circular reference, the default value is 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | True if calculations in this workbook will be done using only the precision of the numbers as they're displayed |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | Indicates whether re-calculate all formulas on opening file. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | Sets the author of the file. |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | Indicates whether checking custom number format when setting Style.Custom, default is false. |
| [setCheckExcelRestriction(boolean value)](#setCheckExcelRestriction-boolean-) | Whether check restriction of excel file when user modify cells related objects. |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | Indicates whether create calculated formulas chain. |
| [setDate1904(boolean value)](#setDate1904-boolean-) | Sets a value which represents if the workbook uses the 1904 date system. |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | Indicates whether fully calculates every time when a calculation is triggered. |
| [setIteration(boolean value)](#setIteration-boolean-) | Indicates whether use iteration to resolve circular references. |
| [setMaxIteration(int value)](#setMaxIteration-int-) | Returns or sets the maximum number of iterations to resolve a circular reference, the default value is 100. |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | True if calculations in this workbook will be done using only the precision of the numbers as they're displayed |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | Indicates whether re-calculate all formulas on opening file. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridWorkbookSettings() {#GridWorkbookSettings--}
```
public GridWorkbookSettings()
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
### getAuthor() {#getAuthor--}
```
public String getAuthor()
```


Gets the author of the file.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


Indicates whether checking custom number format when setting Style.Custom, default is false.

**Returns:**
boolean
### getCheckExcelRestriction() {#getCheckExcelRestriction--}
```
public boolean getCheckExcelRestriction()
```


Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. default is false.

**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getCreateCalcChain() {#getCreateCalcChain--}
```
public boolean getCreateCalcChain()
```


Indicates whether create calculated formulas chain. Default is false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


Gets a value which represents if the workbook uses the 1904 date system.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


Indicates whether fully calculates every time when a calculation is triggered.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


Indicates whether use iteration to resolve circular references.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


Returns or sets the maximum number of iterations to resolve a circular reference, the default value is 100.

**Returns:**
int
### getPrecisionAsDisplayed() {#getPrecisionAsDisplayed--}
```
public boolean getPrecisionAsDisplayed()
```


True if calculations in this workbook will be done using only the precision of the numbers as they're displayed

**Returns:**
boolean
### getReCalculateOnOpen() {#getReCalculateOnOpen--}
```
public boolean getReCalculateOnOpen()
```


Indicates whether re-calculate all formulas on opening file. Default is true.

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




### setAuthor(String value) {#setAuthor-java.lang.String-}
```
public void setAuthor(String value)
```


Sets the author of the file.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


Indicates whether checking custom number format when setting Style.Custom, default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCheckExcelRestriction(boolean value) {#setCheckExcelRestriction-boolean-}
```
public void setCheckExcelRestriction(boolean value)
```


Whether check restriction of excel file when user modify cells related objects. For example, excel does not allow inputting string value longer than 32K. When you input a value longer than 32K such as by Cell.PutValue(string), if this property is true, you will get an Exception. If this property is false, we will accept your input string value as the cell's value so that later you can output the complete string value for other file formats such as CSV. However, if you have set such kind of value that is invalid for excel file format, you should not save the workbook as excel file format later. Otherwise there may be unexpected error for the generated excel file. default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


Indicates whether create calculated formulas chain. Default is false.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


Sets a value which represents if the workbook uses the 1904 date system.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


Enable macros; Now it only works when copying a worksheet to other worksheet in a workbook.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


Indicates whether fully calculates every time when a calculation is triggered.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


Indicates whether use iteration to resolve circular references.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


Returns or sets the maximum number of iterations to resolve a circular reference, the default value is 100.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


True if calculations in this workbook will be done using only the precision of the numbers as they're displayed

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


Indicates whether re-calculate all formulas on opening file. Default is true.

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

