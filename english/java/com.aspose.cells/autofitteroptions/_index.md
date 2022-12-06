---
title: AutoFitterOptions
second_title: Aspose.Cells for Java API Reference
description: Represents all auto fitter options.
type: docs
url: /java/com.aspose.cells/autofitteroptions/
---

**Inheritance:**
java.lang.Object
```
public class AutoFitterOptions
```

Represents all auto fitter options.
## Constructors

| Constructor | Description |
| --- | --- |
| [AutoFitterOptions()](#AutoFitterOptions--) |  |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoFitMergedCells()](#getAutoFitMergedCells--) | Indicates whether auto fit row height when the cells is merged in a row. |
| [getAutoFitMergedCellsType()](#getAutoFitMergedCellsType--) | the type of auto fitting row height of merged cells. |
| [getAutoFitWrappedTextType()](#getAutoFitWrappedTextType--) | the type of auto fitting wrapped text. |
| [getClass()](#getClass--) |  |
| [getDefaultEditLanguage()](#getDefaultEditLanguage--) | default edit language. |
| [getFormatStrategy()](#getFormatStrategy--) | the formatted strategy. |
| [getIgnoreHidden()](#getIgnoreHidden--) | Ignores the hidden rows/columns. |
| [getMaxRowHeight()](#getMaxRowHeight--) | the max row height(in unit of Point) when autofitting rows. |
| [getOnlyAuto()](#getOnlyAuto--) | Indicates whether only fit the rows which height are not customed. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoFitMergedCells(boolean value)](#setAutoFitMergedCells-boolean-) | For the description of this property, please see [getAutoFitMergedCells()](../../com.aspose.cells/autofitteroptions\#getAutoFitMergedCells--) |
| [setAutoFitMergedCellsType(int value)](#setAutoFitMergedCellsType-int-) | For the description of this property, please see [getAutoFitMergedCellsType()](../../com.aspose.cells/autofitteroptions\#getAutoFitMergedCellsType--) |
| [setAutoFitWrappedTextType(int value)](#setAutoFitWrappedTextType-int-) | For the description of this property, please see [getAutoFitWrappedTextType()](../../com.aspose.cells/autofitteroptions\#getAutoFitWrappedTextType--) |
| [setDefaultEditLanguage(int value)](#setDefaultEditLanguage-int-) | For the description of this property, please see [getDefaultEditLanguage()](../../com.aspose.cells/autofitteroptions\#getDefaultEditLanguage--) |
| [setFormatStrategy(int value)](#setFormatStrategy-int-) | For the description of this property, please see [getFormatStrategy()](../../com.aspose.cells/autofitteroptions\#getFormatStrategy--) |
| [setIgnoreHidden(boolean value)](#setIgnoreHidden-boolean-) | For the description of this property, please see [getIgnoreHidden()](../../com.aspose.cells/autofitteroptions\#getIgnoreHidden--) |
| [setMaxRowHeight(double value)](#setMaxRowHeight-double-) | For the description of this property, please see [getMaxRowHeight()](../../com.aspose.cells/autofitteroptions\#getMaxRowHeight--) |
| [setOnlyAuto(boolean value)](#setOnlyAuto-boolean-) | For the description of this property, please see [getOnlyAuto()](../../com.aspose.cells/autofitteroptions\#getOnlyAuto--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### AutoFitterOptions() {#AutoFitterOptions--}
```
public AutoFitterOptions()
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
### getAutoFitMergedCells() {#getAutoFitMergedCells--}
```
public boolean getAutoFitMergedCells()
```


Indicates whether auto fit row height when the cells is merged in a row. The default value is false. NOTE: This member is now obsolete. Instead, please use AutoFitterOptions.AutoFitMergedCellsType property, instead. This property will be removed 12 months later since December 2018. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
boolean
### getAutoFitMergedCellsType() {#getAutoFitMergedCellsType--}
```
public int getAutoFitMergedCellsType()
```


the type of auto fitting row height of merged cells. Excel defaults to ignore merged cells when fitting the row height, so Aspose.Cells works as MS Excel default. Please set this type to change the way of auto fitting row height of merged cells.

**Returns:**
int
### getAutoFitWrappedTextType() {#getAutoFitWrappedTextType--}
```
public int getAutoFitWrappedTextType()
```


the type of auto fitting wrapped text.

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDefaultEditLanguage() {#getDefaultEditLanguage--}
```
public int getDefaultEditLanguage()
```


default edit language. It may display/render different layouts for text paragraph when different edit languages is set. Default is DefaultEditLanguage.AUTO.

**Returns:**
int
### getFormatStrategy() {#getFormatStrategy--}
```
public int getFormatStrategy()
```


the formatted strategy. The default value is CellStyle for performance.

**Returns:**
int
### getIgnoreHidden() {#getIgnoreHidden--}
```
public boolean getIgnoreHidden()
```


Ignores the hidden rows/columns.

**Returns:**
boolean
### getMaxRowHeight() {#getMaxRowHeight--}
```
public double getMaxRowHeight()
```


the max row height(in unit of Point) when autofitting rows.

**Returns:**
double
### getOnlyAuto() {#getOnlyAuto--}
```
public boolean getOnlyAuto()
```


Indicates whether only fit the rows which height are not customed.

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




### setAutoFitMergedCells(boolean value) {#setAutoFitMergedCells-boolean-}
```
public void setAutoFitMergedCells(boolean value)
```


For the description of this property, please see [getAutoFitMergedCells()](../../com.aspose.cells/autofitteroptions\#getAutoFitMergedCells--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutoFitMergedCellsType(int value) {#setAutoFitMergedCellsType-int-}
```
public void setAutoFitMergedCellsType(int value)
```


For the description of this property, please see [getAutoFitMergedCellsType()](../../com.aspose.cells/autofitteroptions\#getAutoFitMergedCellsType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setAutoFitWrappedTextType(int value) {#setAutoFitWrappedTextType-int-}
```
public void setAutoFitWrappedTextType(int value)
```


For the description of this property, please see [getAutoFitWrappedTextType()](../../com.aspose.cells/autofitteroptions\#getAutoFitWrappedTextType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDefaultEditLanguage(int value) {#setDefaultEditLanguage-int-}
```
public void setDefaultEditLanguage(int value)
```


For the description of this property, please see [getDefaultEditLanguage()](../../com.aspose.cells/autofitteroptions\#getDefaultEditLanguage--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setFormatStrategy(int value) {#setFormatStrategy-int-}
```
public void setFormatStrategy(int value)
```


For the description of this property, please see [getFormatStrategy()](../../com.aspose.cells/autofitteroptions\#getFormatStrategy--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setIgnoreHidden(boolean value) {#setIgnoreHidden-boolean-}
```
public void setIgnoreHidden(boolean value)
```


For the description of this property, please see [getIgnoreHidden()](../../com.aspose.cells/autofitteroptions\#getIgnoreHidden--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setMaxRowHeight(double value) {#setMaxRowHeight-double-}
```
public void setMaxRowHeight(double value)
```


For the description of this property, please see [getMaxRowHeight()](../../com.aspose.cells/autofitteroptions\#getMaxRowHeight--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |

### setOnlyAuto(boolean value) {#setOnlyAuto-boolean-}
```
public void setOnlyAuto(boolean value)
```


For the description of this property, please see [getOnlyAuto()](../../com.aspose.cells/autofitteroptions\#getOnlyAuto--)

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

