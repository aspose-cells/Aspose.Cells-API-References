##DefaultStyleSettings
Settings for the default values of workbooks style properties.
**Inheritance:**
java.lang.Object
```
public class DefaultStyleSettings
```
Settings for the default values of workbook's style properties.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBuiltInPreference()](#getBuiltInPreference--) | Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. |
| [getClass()](#getClass--) |  |
| [getFontName()](#getFontName--) | Gets the default font name for the workbook |
| [getFontSize()](#getFontSize--) | Gets the default standard font size for the workbook. |
| [getHorizontalAlignment()](#getHorizontalAlignment--) | Gets the default value for horizontal alignment |
| [getVerticalAlignment()](#getVerticalAlignment--) | Gets the default value for vertical alignment |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setBuiltInPreference(boolean value)](#setBuiltInPreference-boolean-) | Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. |
| [setFontName(String value)](#setFontName-java.lang.String-) | Sets the default font name for the workbook |
| [setFontSize(double value)](#setFontSize-double-) | Sets the default standard font size for the workbook. |
| [setHorizontalAlignment(int value)](#setHorizontalAlignment-int-) | Sets the default value for horizontal alignment |
| [setVerticalAlignment(int value)](#setVerticalAlignment-int-) | Sets the default value for vertical alignment |
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
### getBuiltInPreference() {#getBuiltInPreference--}
```
public boolean getBuiltInPreference()
```
Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.
**Remarks**
When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFontName() {#getFontName--}
```
public String getFontName()
```
Gets the default font name for the workbook
**Returns:**
java.lang.String
### getFontSize() {#getFontSize--}
```
public double getFontSize()
```
Gets the default standard font size for the workbook.
**Returns:**
double
### getHorizontalAlignment() {#getHorizontalAlignment--}
```
public int getHorizontalAlignment()
```
Gets the default value for horizontal alignment
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Returns:**
int
### getVerticalAlignment() {#getVerticalAlignment--}
```
public int getVerticalAlignment()
```
Gets the default value for vertical alignment
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Returns:**
int
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
### setBuiltInPreference(boolean value) {#setBuiltInPreference-boolean-}
```
public void setBuiltInPreference(boolean value)
```
Indicates whether property for number format is preferable when the style defines both built-in number and custom pattern. Default value is false, that means by default custom pattern will be used to format values as long as it is not empty for one style.
**Remarks**
When loading workbook from existing template file, maybe both built-in number and custom pattern are defined for one style. This property determine whether we should use the built-in number or the custom pattern when formatting values with the style.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setFontName(String value) {#setFontName-java.lang.String-}
```
public void setFontName(String value)
```
Sets the default font name for the workbook
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFontSize(double value) {#setFontSize-double-}
```
public void setFontSize(double value)
```
Sets the default standard font size for the workbook.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | double |  |
### setHorizontalAlignment(int value) {#setHorizontalAlignment-int-}
```
public void setHorizontalAlignment(int value)
```
Sets the default value for horizontal alignment
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setVerticalAlignment(int value) {#setVerticalAlignment-int-}
```
public void setVerticalAlignment(int value)
```
Sets the default value for vertical alignment
See [TextAlignmentType](../../com.aspose.cells/textalignmenttype).
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
