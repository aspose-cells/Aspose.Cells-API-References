---
title: CopyOptions
second_title: Aspose.Cells for Java API Reference
description: Represents the copy options.
type: docs
weight: 133
url: /java/com.aspose.cells/copyoptions/
---

**Inheritance:**
java.lang.Object
```
public class CopyOptions
```

Represents the copy options.
## Constructors

| Constructor | Description |
| --- | --- |
| [CopyOptions()](#CopyOptions--) | CopyOptions constructor. |
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getColumnCharacterWidth()](#getColumnCharacterWidth--) | Indicates whether copying column width in unit of characters. |
| [getCopyInvalidFormulasAsValues()](#getCopyInvalidFormulasAsValues--) | If the formula is not valid for the dest destination, only copy values. |
| [getCopyNames()](#getCopyNames--) | Indicates whether copying the names. |
| [getExtendToAdjacentRange()](#getExtendToAdjacentRange--) | Indicates whether extend ranges when copying the range to adjacent range. |
| [getKeepMacros()](#getKeepMacros--) | Indicates whether keeping macros; Only for copying workbook. |
| [getReferToDestinationSheet()](#getReferToDestinationSheet--) | When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. |
| [getReferToSheetWithSameName()](#getReferToSheetWithSameName--) | When copying a worksheet to another workbook and the worksheet contains the formulas which refer to other worksheets in MS Excel, the copied formulas should refer to source workbook. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setColumnCharacterWidth(boolean value)](#setColumnCharacterWidth-boolean-) | For the description of this property, please see \#getColumnCharacterWidth().getColumnCharacterWidth() |
| [setCopyInvalidFormulasAsValues(boolean value)](#setCopyInvalidFormulasAsValues-boolean-) | For the description of this property, please see \#getCopyInvalidFormulasAsValues().getCopyInvalidFormulasAsValues() |
| [setCopyNames(boolean value)](#setCopyNames-boolean-) | For the description of this property, please see \#getCopyNames().getCopyNames() |
| [setExtendToAdjacentRange(boolean value)](#setExtendToAdjacentRange-boolean-) | For the description of this property, please see \#getExtendToAdjacentRange().getExtendToAdjacentRange() |
| [setKeepMacros(boolean value)](#setKeepMacros-boolean-) | For the description of this property, please see \#getKeepMacros().getKeepMacros() |
| [setReferToDestinationSheet(boolean value)](#setReferToDestinationSheet-boolean-) | For the description of this property, please see \#getReferToDestinationSheet().getReferToDestinationSheet() |
| [setReferToSheetWithSameName(boolean value)](#setReferToSheetWithSameName-boolean-) | For the description of this property, please see \#getReferToSheetWithSameName().getReferToSheetWithSameName() |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CopyOptions() {#CopyOptions--}
```
public CopyOptions()
```


CopyOptions constructor.

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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getColumnCharacterWidth() {#getColumnCharacterWidth--}
```
public boolean getColumnCharacterWidth()
```


Indicates whether copying column width in unit of characters.

**Returns:**
boolean
### getCopyInvalidFormulasAsValues() {#getCopyInvalidFormulasAsValues--}
```
public boolean getCopyInvalidFormulasAsValues()
```


If the formula is not valid for the dest destination, only copy values.

**Returns:**
boolean
### getCopyNames() {#getCopyNames--}
```
public boolean getCopyNames()
```


Indicates whether copying the names.

**Returns:**
boolean
### getExtendToAdjacentRange() {#getExtendToAdjacentRange--}
```
public boolean getExtendToAdjacentRange()
```


Indicates whether extend ranges when copying the range to adjacent range. If it's true, only extends the range of the hyperlink,not adding a new hyperlink when copying hyperlinks to adjacent rows.

**Returns:**
boolean
### getKeepMacros() {#getKeepMacros--}
```
public boolean getKeepMacros()
```


Indicates whether keeping macros; Only for copying workbook.

**Returns:**
boolean
### getReferToDestinationSheet() {#getReferToDestinationSheet--}
```
public boolean getReferToDestinationSheet()
```


When copying the range in the same file and the chart refers to the source sheet, False means the copied chart's data source will not be changed. True means the copied chart's data source refers to the destination sheet. The default value is false, it works as MS Excel.

**Returns:**
boolean
### getReferToSheetWithSameName() {#getReferToSheetWithSameName--}
```
public boolean getReferToSheetWithSameName()
```


When copying a worksheet to another workbook and the worksheet contains the formulas which refer to other worksheets in MS Excel, the copied formulas should refer to source workbook. But sometimes we have copied other worksheets and we hope the copied formulas refer to other worksheets with the name in the same workbook, please set this property as true. The default value is true.

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




### setColumnCharacterWidth(boolean value) {#setColumnCharacterWidth-boolean-}
```
public void setColumnCharacterWidth(boolean value)
```


For the description of this property, please see \#getColumnCharacterWidth().getColumnCharacterWidth()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCopyInvalidFormulasAsValues(boolean value) {#setCopyInvalidFormulasAsValues-boolean-}
```
public void setCopyInvalidFormulasAsValues(boolean value)
```


For the description of this property, please see \#getCopyInvalidFormulasAsValues().getCopyInvalidFormulasAsValues()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setCopyNames(boolean value) {#setCopyNames-boolean-}
```
public void setCopyNames(boolean value)
```


For the description of this property, please see \#getCopyNames().getCopyNames()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setExtendToAdjacentRange(boolean value) {#setExtendToAdjacentRange-boolean-}
```
public void setExtendToAdjacentRange(boolean value)
```


For the description of this property, please see \#getExtendToAdjacentRange().getExtendToAdjacentRange()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setKeepMacros(boolean value) {#setKeepMacros-boolean-}
```
public void setKeepMacros(boolean value)
```


For the description of this property, please see \#getKeepMacros().getKeepMacros()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setReferToDestinationSheet(boolean value) {#setReferToDestinationSheet-boolean-}
```
public void setReferToDestinationSheet(boolean value)
```


For the description of this property, please see \#getReferToDestinationSheet().getReferToDestinationSheet()

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setReferToSheetWithSameName(boolean value) {#setReferToSheetWithSameName-boolean-}
```
public void setReferToSheetWithSameName(boolean value)
```


For the description of this property, please see \#getReferToSheetWithSameName().getReferToSheetWithSameName()

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

