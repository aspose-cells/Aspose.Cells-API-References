##TickLabels
Represents the tick-mark labels associated with tick marks on a chart axis.
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
| [getAlignmentType()](#getAlignmentType--) | Gets the text alignment for the tick labels on the axis. |
| [getAutoScaleFont()](#getAutoScaleFont--) | True if the text in the object changes font size when the object size changes. |
| [getBackgroundMode()](#getBackgroundMode--) | Gets the display mode of the background |
| [getClass()](#getClass--) |  |
| [getDirectionType()](#getDirectionType--) | Gets the direction of text. |
| [getDisplayNumberFormat()](#getDisplayNumberFormat--) | Gets the display number format of tick labels. |
| [getFont()](#getFont--) | Returns a [ChartArea.getFont()](../../com.aspose.cells/chartarea\#getFont--) object that represents the font of the specified TickLabels object. |
| [getNumber()](#getNumber--) | Represents the format number for the TickLabels object. |
| [getNumberFormat()](#getNumberFormat--) | Represents the format string for the TickLabels object. |
| [getNumberFormatLinked()](#getNumberFormatLinked--) | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [getOffset()](#getOffset--) | Gets the distance of labels from the category axis. |
| [getReadingOrder()](#getReadingOrder--) | Represents text reading order. |
| [getRotationAngle()](#getRotationAngle--) | Represents text rotation angle in clockwise. |
| [getTextDirection()](#getTextDirection--) | Represents text reading order. |
| [getTickLabelItems()](#getTickLabelItems--) | Gets the display tick labels of the axis. |
| [hashCode()](#hashCode--) |  |
| [isAutomaticRotation()](#isAutomaticRotation--) | Indicates whether the rotation angle is automatic |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAlignmentType(int value)](#setAlignmentType-int-) | Sets the text alignment for the tick labels on the axis. |
| [setAutoScaleFont(boolean value)](#setAutoScaleFont-boolean-) | True if the text in the object changes font size when the object size changes. |
| [setAutomaticRotation(boolean value)](#setAutomaticRotation-boolean-) | Indicates whether the rotation angle is automatic |
| [setBackgroundMode(int value)](#setBackgroundMode-int-) | Sets the display mode of the background |
| [setDirectionType(int value)](#setDirectionType-int-) | Sets the direction of text. |
| [setNumber(int value)](#setNumber-int-) | Represents the format number for the TickLabels object. |
| [setNumberFormat(String value)](#setNumberFormat-java.lang.String-) | Represents the format string for the TickLabels object. |
| [setNumberFormatLinked(boolean value)](#setNumberFormatLinked-boolean-) | True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells). |
| [setOffset(int value)](#setOffset-int-) | Sets the distance of labels from the category axis. |
| [setReadingOrder(int value)](#setReadingOrder-int-) | Represents text reading order. |
| [setRotationAngle(int value)](#setRotationAngle-int-) | Represents text rotation angle in clockwise. |
| [setTextDirection(int value)](#setTextDirection-int-) | Represents text reading order. |
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
### getAlignmentType() {#getAlignmentType--}
```
public int getAlignmentType()
```
Gets the text alignment for the tick labels on the axis.
See [TickLabelAlignmentType](../../com.aspose.cells/ticklabelalignmenttype).
**Returns:**
int
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
Gets the display mode of the background
See [BackgroundMode](../../com.aspose.cells/backgroundmode).
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
Gets the direction of text.
See [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).
**Returns:**
int
### getDisplayNumberFormat() {#getDisplayNumberFormat--}
```
public String getDisplayNumberFormat()
```
Gets the display number format of tick labels.
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
Represents the format string for the TickLabels object.
**Remarks**
The formatting string is same as a custom format string setting to a cell. For example, "$0".
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
Gets the distance of labels from the category axis. Only for category (x) axis.
**Remarks**
The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label''s font size.
**Returns:**
int
### getReadingOrder() {#getReadingOrder--}
```
public int getReadingOrder()
```
Represents text reading order.
See [TextDirectionType](../../com.aspose.cells/textdirectiontype).
**Returns:**
int
### getRotationAngle() {#getRotationAngle--}
```
public int getRotationAngle()
```
Represents text rotation angle in clockwise.
**Remarks**
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
Represents text reading order.
See [TextDirectionType](../../com.aspose.cells/textdirectiontype).
**Remarks**
NOTE: This member is now obsolete. Instead, please use TickLabels.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
int
### getTickLabelItems() {#getTickLabelItems--}
```
public TickLabelItem[] getTickLabelItems()
```
Gets the display tick labels of the axis.
**Remarks**
Only available after calling [Chart.calculate()](../../com.aspose.cells/chart\#calculate--) method.
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
### setAlignmentType(int value) {#setAlignmentType-int-}
```
public void setAlignmentType(int value)
```
Sets the text alignment for the tick labels on the axis.
See [TickLabelAlignmentType](../../com.aspose.cells/ticklabelalignmenttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setAutoScaleFont(boolean value) {#setAutoScaleFont-boolean-}
```
public void setAutoScaleFont(boolean value)
```
True if the text in the object changes font size when the object size changes. The default value is True.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAutomaticRotation(boolean value) {#setAutomaticRotation-boolean-}
```
public void setAutomaticRotation(boolean value)
```
Indicates whether the rotation angle is automatic
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setBackgroundMode(int value) {#setBackgroundMode-int-}
```
public void setBackgroundMode(int value)
```
Sets the display mode of the background
See [BackgroundMode](../../com.aspose.cells/backgroundmode).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setDirectionType(int value) {#setDirectionType-int-}
```
public void setDirectionType(int value)
```
Sets the direction of text.
See [ChartTextDirectionType](../../com.aspose.cells/charttextdirectiontype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setNumber(int value) {#setNumber-int-}
```
public void setNumber(int value)
```
Represents the format number for the TickLabels object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setNumberFormat(String value) {#setNumberFormat-java.lang.String-}
```
public void setNumberFormat(String value)
```
Represents the format string for the TickLabels object.
**Remarks**
The formatting string is same as a custom format string setting to a cell. For example, "$0".
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setNumberFormatLinked(boolean value) {#setNumberFormatLinked-boolean-}
```
public void setNumberFormatLinked(boolean value)
```
True if the number format is linked to the cells (so that the number format changes in the labels when it changes in the cells).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setOffset(int value) {#setOffset-int-}
```
public void setOffset(int value)
```
Sets the distance of labels from the category axis. Only for category (x) axis.
**Remarks**
The default distance is 100 percent, which represents the default spacing between the axis labels and the axis line. The value can be an integer percentage from 0 through 1000, relative to the axis label''s font size.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setReadingOrder(int value) {#setReadingOrder-int-}
```
public void setReadingOrder(int value)
```
Represents text reading order.
See [TextDirectionType](../../com.aspose.cells/textdirectiontype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRotationAngle(int value) {#setRotationAngle-int-}
```
public void setRotationAngle(int value)
```
Represents text rotation angle in clockwise.
**Remarks**
0: Not rotated.
255: Top to Bottom.
\-90: Downward.
90: Upward.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setTextDirection(int value) {#setTextDirection-int-}
```
public void setTextDirection(int value)
```
Represents text reading order.
See [TextDirectionType](../../com.aspose.cells/textdirectiontype).
**Remarks**
NOTE: This member is now obsolete. Instead, please use TickLabels.ReadingOrder property. This property will be removed 12 months later since March 2020. Aspose apologizes for any inconvenience you may have experienced.
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
