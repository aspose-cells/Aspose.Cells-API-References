---
title: TickLabels
second_title: Aspose.Cells for Java API Reference
description: Represents the tick-mark labels associated with tick marks on a chart axis.
type: docs
weight: 598
url: /java/com.aspose.cells/ticklabels/
---

**Inheritance:**
java.lang.Object
```
public class TickLabels
```

Represents the tick-mark labels associated with tick marks on a chart axis.
## Methods

| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAutoScaleFont()](#getAutoScaleFont--) | True if the text in the object changes font size when the object size changes. |
| [getBackgroundMode()](#getBackgroundMode--) | Gets and sets the display mode of the background |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Gets and sets the direction of text. |
| [getDisplayNumberFormat()](#getDisplayNumberFormat--) | Gets and sets the display number format of tick labels. |
| [getFont()](#getFont--) | Returns a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object that represents the font of the specified TickLabels object. |
| [getNumber()](#getNumber--) | Represents the format number for the TickLabels object. |
| [getNumberFormat()](#getNumberFormat--) | Represents the format string for the TickLabels object. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [getOffset()](#getOffset--) | Gets and sets the distance of labels from the axis. |
| [getReadingOrder()](#getReadingOrder--) | Represents text reading order. |
| [getRotationAngle()](#getRotationAngle--) | Represents text rotation angle in clockwise. |
| [getTextDirection()](#getTextDirection--) | Represents text reading order. |
| [getTickLabelItems()](#getTickLabelItems--) | Gets the items' info of TickLabel. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indicates whether the rotation angle is automatic |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | Please see the getter of this property: [getAutoScaleFont()](../../com.aspose.cells/ticklabels\#getAutoScaleFont--) |
| [setAutomaticRotation(boolean value)](#setAutomaticRotation-boolean-) | Please see the getter of this property: [isAutomaticRotation()](../../com.aspose.cells/ticklabels\#isAutomaticRotation--) |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Please see the getter of this property: [getBackgroundMode()](../../com.aspose.cells/ticklabels\#getBackgroundMode--) |
| [setDirectionType(int value)](#setDirectionType-int-) | Please see the getter of this property: [getDirectionType()](../../com.aspose.cells/ticklabels\#getDirectionType--) |
| [setNumber(int value)](#setNumber-int-) | Please see the getter of this property: [getNumber()](../../com.aspose.cells/ticklabels\#getNumber--) |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Please see the getter of this property: [getNumberFormat()](../../com.aspose.cells/ticklabels\#getNumberFormat--) |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | Please see the getter of this property: [getNumberFormatLinked()](../../com.aspose.cells/ticklabels\#getNumberFormatLinked--) |
| [setOffset(int value)](#setOffset-int-) | Please see the getter of this property: [getOffset()](../../com.aspose.cells/ticklabels\#getOffset--) |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Please see the getter of this property: [getReadingOrder()](../../com.aspose.cells/ticklabels\#getReadingOrder--) |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Please see the getter of this property: [getRotationAngle()](../../com.aspose.cells/ticklabels\#getRotationAngle--) |
| [setTextDirection(int value)](#setTextDirection-int-) | Please see the getter of this property: [getTextDirection()](../../com.aspose.cells/ticklabels\#getTextDirection--) |
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
### getAutoScaleFont() {#getAutoScaleFont--}
```
public boolean getAutoScaleFont()
```


True if the text in the object changes font size when the object size changes. The default value is True.

**Returns:**
boolean
### getBackgroundMode() {#getBackgroundMode--}
```
public int getBackgroundMode()
```


Gets and sets the display mode of the background

**Returns:**
int
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```




**Returns:**
java.lang.Class<?>
### getDirectionType() {#getDirectionType--}
```
public int getDirectionType()
```


Gets and sets the direction of text.

**Returns:**
int
### getDisplayNumberFormat() {#getDisplayNumberFormat--}
```
public String getDisplayNumberFormat()
```


Gets and sets the display number format of tick labels.

**Returns:**
java.lang.String
### getFont() {#getFont--}
```
public Font getFont()
```


Returns a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object that represents the font of the specified TickLabels object.

**Returns:**
[Font](../../com.aspose.cells/font)
### getNumber() {#getNumber--}
```
public int getNumber()
```


Represents the format number for the TickLabels object.

**Returns:**
int
### getNumberFormat() {#getNumberFormat--}
```
public String getNumberFormat()
```


Represents the format string for the TickLabels object. The formatting string is same as a custom format string setting to a cell. For example, "$0".

**Returns:**
java.lang.String
### getNumberFormatLinked() {#getNumberFormatLinked--}
```
public boolean getNumberFormatLinked()
```


True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).

**Returns:**
boolean
### getOffset() {#getOffset--}
```
public int getOffset()
```


Gets and sets the distance of labels from the axis. The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label\\u9225\\u6a9a font size.

**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```


Represents text reading order.

**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```


Represents text rotation angle in clockwise.
0: Not rotated.

255: Top to Bottom.

\-90: Downward.

90: Upward.


**Returns:**
int
### getTextDirection() {#getTextDirection--}
```
public int getTextDirection()
```


Represents text reading order. NOTE: This member is now obsolete. Instead, please use TickLabels.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.

**Returns:**
int
### getTickLabelItems() {#getTickLabelItems--}
```
public TickLabelItem[] getTickLabelItems()
```


Gets the items' info of TickLabel. Only exists after calling [Chart.calculate()](../../com.aspose.cells/chart\#calculate--) method.

**Returns:**
com.aspose.cells.TickLabelItem[]
### hashCode() {#hashCode--}
```
public native int hashCode()
```




**Returns:**
int
### isAutomaticRotation() {#isAutomaticRotation--}
```
public boolean isAutomaticRotation()
```


Indicates whether the rotation angle is automatic

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




### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```


Please see the getter of this property: [getAutoScaleFont()](../../com.aspose.cells/ticklabels\#getAutoScaleFont--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setAutomaticRotation(boolean value) {#setAutomaticRotation-boolean-}
```
public void setAutomaticRotation(boolean value)
```


Please see the getter of this property: [isAutomaticRotation()](../../com.aspose.cells/ticklabels\#isAutomaticRotation--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```


Please see the getter of this property: [getBackgroundMode()](../../com.aspose.cells/ticklabels\#getBackgroundMode--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```


Please see the getter of this property: [getDirectionType()](../../com.aspose.cells/ticklabels\#getDirectionType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```


Please see the getter of this property: [getNumber()](../../com.aspose.cells/ticklabels\#getNumber--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```


Please see the getter of this property: [getNumberFormat()](../../com.aspose.cells/ticklabels\#getNumberFormat--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```


Please see the getter of this property: [getNumberFormatLinked()](../../com.aspose.cells/ticklabels\#getNumberFormatLinked--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setOffset(int value) {#setOffset-int-}
```
public void setOffset(int value)
```


Please see the getter of this property: [getOffset()](../../com.aspose.cells/ticklabels\#getOffset--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```


Please see the getter of this property: [getReadingOrder()](../../com.aspose.cells/ticklabels\#getReadingOrder--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```


Please see the getter of this property: [getRotationAngle()](../../com.aspose.cells/ticklabels\#getRotationAngle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```


Please see the getter of this property: [getTextDirection()](../../com.aspose.cells/ticklabels\#getTextDirection--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

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

