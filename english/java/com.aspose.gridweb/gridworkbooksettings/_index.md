---
title: GridWorkbookSettings
second_title: Aspose.Cells for Java API Reference
description: Represents   settings of the workbook.
type: docs
url: /java/com.aspose.gridweb/gridworkbooksettings/
---

**Inheritance:**
java.lang.Object
```
public class GridWorkbookSettings
```

Represents settings of the workbook.

```
GridWeb gridweb = new GridWeb();
         GridWorkbookSettings gsettings = new GridWorkbookSettings();
         gridweb.setSettings(gsettings);
 
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
| [getAuthor()](#getAuthor--) | the author of the file. |
| [getCheckCustomNumberFormat()](#getCheckCustomNumberFormat--) | whether checking custom number format when setting Style.Custom. |
| [getClass()](#getClass--) |  |
| [getCreateCalcChain()](#getCreateCalcChain--) | whether create calculated formulas chain. |
| [getDate1904()](#getDate1904--) | the value which represents if the workbook uses the 1904 date system. |
| [getEnableMacros()](#getEnableMacros--) | whether enable macros; Now it only works when copying a worksheet to other worksheet in a workbook. |
| [getForceFullCalculate()](#getForceFullCalculate--) | whether fully calculates every time when a calculation is triggered. |
| [getIteration()](#getIteration--) | whether use iteration to resolve circular references. |
| [getMaxIteration()](#getMaxIteration--) | the maximum number of iterations to resolve a circular reference,the default value is 100. |
| [getPrecisionAsDisplayed()](#getPrecisionAsDisplayed--) | True if calculations in this workbook will be done using only the precision of the numbers as they're displayed |
| [getReCalculateOnOpen()](#getReCalculateOnOpen--) | whether re-calculate all formulas on opening file. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAuthor(String value)](#setAuthor-java.lang.String-) | For the description of this property, please see [getAuthor()](../../com.aspose.gridweb/gridworkbooksettings\#getAuthor--) |
| [setCheckCustomNumberFormat(boolean value)](#setCheckCustomNumberFormat-boolean-) | For the description of this property, please see [getCheckCustomNumberFormat()](../../com.aspose.gridweb/gridworkbooksettings\#getCheckCustomNumberFormat--) |
| [setCreateCalcChain(boolean value)](#setCreateCalcChain-boolean-) | For the description of this property, please see [getCreateCalcChain()](../../com.aspose.gridweb/gridworkbooksettings\#getCreateCalcChain--) |
| [setDate1904(boolean value)](#setDate1904-boolean-) | For the description of this property, please see [getDate1904()](../../com.aspose.gridweb/gridworkbooksettings\#getDate1904--) |
| [setEnableMacros(boolean value)](#setEnableMacros-boolean-) | For the description of this property, please see [getEnableMacros()](../../com.aspose.gridweb/gridworkbooksettings\#getEnableMacros--) |
| [setForceFullCalculate(boolean value)](#setForceFullCalculate-boolean-) | For the description of this property, please see [getForceFullCalculate()](../../com.aspose.gridweb/gridworkbooksettings\#getForceFullCalculate--) |
| [setIteration(boolean value)](#setIteration-boolean-) | For the description of this property, please see [getIteration()](../../com.aspose.gridweb/gridworkbooksettings\#getIteration--) |
| [setMaxIteration(int value)](#setMaxIteration-int-) | For the description of this property, please see [getMaxIteration()](../../com.aspose.gridweb/gridworkbooksettings\#getMaxIteration--) |
| [setPrecisionAsDisplayed(boolean value)](#setPrecisionAsDisplayed-boolean-) | For the description of this property, please see [getPrecisionAsDisplayed()](../../com.aspose.gridweb/gridworkbooksettings\#getPrecisionAsDisplayed--) |
| [setReCalculateOnOpen(boolean value)](#setReCalculateOnOpen-boolean-) | For the description of this property, please see [getReCalculateOnOpen()](../../com.aspose.gridweb/gridworkbooksettings\#getReCalculateOnOpen--) |
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


the author of the file.

**Returns:**
java.lang.String
### getCheckCustomNumberFormat() {#getCheckCustomNumberFormat--}
```
public boolean getCheckCustomNumberFormat()
```


whether checking custom number format when setting Style.Custom.

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


whether create calculated formulas chain. Default is false.

**Returns:**
boolean
### getDate1904() {#getDate1904--}
```
public boolean getDate1904()
```


the value which represents if the workbook uses the 1904 date system.

**Returns:**
boolean
### getEnableMacros() {#getEnableMacros--}
```
public boolean getEnableMacros()
```


whether enable macros; Now it only works when copying a worksheet to other worksheet in a workbook.

**Returns:**
boolean
### getForceFullCalculate() {#getForceFullCalculate--}
```
public boolean getForceFullCalculate()
```


whether fully calculates every time when a calculation is triggered.

**Returns:**
boolean
### getIteration() {#getIteration--}
```
public boolean getIteration()
```


whether use iteration to resolve circular references.

**Returns:**
boolean
### getMaxIteration() {#getMaxIteration--}
```
public int getMaxIteration()
```


the maximum number of iterations to resolve a circular reference,the default value is 100.

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


whether re-calculate all formulas on opening file.

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


For the description of this property, please see [getAuthor()](../../com.aspose.gridweb/gridworkbooksettings\#getAuthor--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setCheckCustomNumberFormat(boolean value) {#setCheckCustomNumberFormat-boolean-}
```
public void setCheckCustomNumberFormat(boolean value)
```


For the description of this property, please see [getCheckCustomNumberFormat()](../../com.aspose.gridweb/gridworkbooksettings\#getCheckCustomNumberFormat--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCreateCalcChain(boolean value) {#setCreateCalcChain-boolean-}
```
public void setCreateCalcChain(boolean value)
```


For the description of this property, please see [getCreateCalcChain()](../../com.aspose.gridweb/gridworkbooksettings\#getCreateCalcChain--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setDate1904(boolean value) {#setDate1904-boolean-}
```
public void setDate1904(boolean value)
```


For the description of this property, please see [getDate1904()](../../com.aspose.gridweb/gridworkbooksettings\#getDate1904--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setEnableMacros(boolean value) {#setEnableMacros-boolean-}
```
public void setEnableMacros(boolean value)
```


For the description of this property, please see [getEnableMacros()](../../com.aspose.gridweb/gridworkbooksettings\#getEnableMacros--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setForceFullCalculate(boolean value) {#setForceFullCalculate-boolean-}
```
public void setForceFullCalculate(boolean value)
```


For the description of this property, please see [getForceFullCalculate()](../../com.aspose.gridweb/gridworkbooksettings\#getForceFullCalculate--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setIteration(boolean value) {#setIteration-boolean-}
```
public void setIteration(boolean value)
```


For the description of this property, please see [getIteration()](../../com.aspose.gridweb/gridworkbooksettings\#getIteration--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMaxIteration(int value) {#setMaxIteration-int-}
```
public void setMaxIteration(int value)
```


For the description of this property, please see [getMaxIteration()](../../com.aspose.gridweb/gridworkbooksettings\#getMaxIteration--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setPrecisionAsDisplayed(boolean value) {#setPrecisionAsDisplayed-boolean-}
```
public void setPrecisionAsDisplayed(boolean value)
```


For the description of this property, please see [getPrecisionAsDisplayed()](../../com.aspose.gridweb/gridworkbooksettings\#getPrecisionAsDisplayed--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setReCalculateOnOpen(boolean value) {#setReCalculateOnOpen-boolean-}
```
public void setReCalculateOnOpen(boolean value)
```


For the description of this property, please see [getReCalculateOnOpen()](../../com.aspose.gridweb/gridworkbooksettings\#getReCalculateOnOpen--)

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

