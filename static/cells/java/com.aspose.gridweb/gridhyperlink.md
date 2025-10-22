##GridHyperlink
Encapsulates the object that represents a hyperlink.
**Inheritance:**
java.lang.Object
```
public class GridHyperlink
```
Encapsulates the object that represents a hyperlink.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Represents the address of a hyperlink. |
| [getAltText()](#getAltText--) | Gets Alternate text for the image link,please note this is an extension attribute and can not keep in excel file |
| [getArea()](#getArea--) | Gets the range of hyperlink. |
| [getClass()](#getClass--) |  |
| [getCommand()](#getCommand--) | Returns or sets the self defined command value text for the specified hyperlink. |
| [getDiscardInput()](#getDiscardInput--) | Indicates whether to discard user input at client browser when user click this CellCommand hyperlink. |
| [getImageURL()](#getImageURL--) | Gets Image URL for the link, there is no imageurl properties in hyperlink, so actually use TextToDisplay to record this value ,TextToDisplay will be set to <img src=value > so it will change the value of TextToDisplay |
| [getScreenTip()](#getScreenTip--) | Returns or sets the ScreenTip text for the specified hyperlink. |
| [getTarget()](#getTarget--) | Gets web link target type,please note this is an extension attribute and can not keep in excel file |
| [getTextToDisplay()](#getTextToDisplay--) | Represents the text to be displayed for the specified hyperlink. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Represents the address of a hyperlink. |
| [setAltText(String value)](#setAltText-java.lang.String-) | Sets Alternate text for the image link,please note this is an extension attribute and can not keep in excel file |
| [setCommand(String value)](#setCommand-java.lang.String-) | Returns or sets the self defined command value text for the specified hyperlink. |
| [setDiscardInput(boolean value)](#setDiscardInput-boolean-) | Indicates whether to discard user input at client browser when user click this CellCommand hyperlink. |
| [setImageURL(String value)](#setImageURL-java.lang.String-) | Sets Image URL for the link, there is no imageurl properties in hyperlink, so actually use TextToDisplay to record this value ,TextToDisplay will be set to <img src=value > so it will change the value of TextToDisplay |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Returns or sets the ScreenTip text for the specified hyperlink. |
| [setTarget(String value)](#setTarget-java.lang.String-) | Sets web link target type,please note this is an extension attribute and can not keep in excel file |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Represents the text to be displayed for the specified hyperlink. |
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
### getAddress() {#getAddress--}
```
public String getAddress()
```
Represents the address of a hyperlink.
**Returns:**
java.lang.String
### getAltText() {#getAltText--}
```
public String getAltText()
```
Gets Alternate text for the image link,please note this is an extension attribute and can not keep in excel file
**Returns:**
java.lang.String
### getArea() {#getArea--}
```
public GridCellArea getArea()
```
Gets the range of hyperlink.
**Returns:**
[GridCellArea](../../com.aspose.gridweb/gridcellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCommand() {#getCommand--}
```
public String getCommand()
```
Returns or sets the self defined command value text for the specified hyperlink.
**Returns:**
java.lang.String
### getDiscardInput() {#getDiscardInput--}
```
public boolean getDiscardInput()
```
Indicates whether to discard user input at client browser when user click this CellCommand hyperlink. Could be used as an "undo" action.
**Returns:**
boolean
### getImageURL() {#getImageURL--}
```
public String getImageURL()
```
Gets Image URL for the link, there is no imageurl properties in hyperlink, so actually use TextToDisplay to record this value ,TextToDisplay will be set to <img src=value > so it will change the value of TextToDisplay
**Returns:**
java.lang.String
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```
Returns or sets the ScreenTip text for the specified hyperlink.
**Returns:**
java.lang.String
### getTarget() {#getTarget--}
```
public String getTarget()
```
Gets web link target type,please note this is an extension attribute and can not keep in excel file
**Returns:**
java.lang.String
### getTextToDisplay() {#getTextToDisplay--}
```
public String getTextToDisplay()
```
Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.
**Returns:**
java.lang.String
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
### setAddress(String value) {#setAddress-java.lang.String-}
```
public void setAddress(String value)
```
Represents the address of a hyperlink.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setAltText(String value) {#setAltText-java.lang.String-}
```
public void setAltText(String value)
```
Sets Alternate text for the image link,please note this is an extension attribute and can not keep in excel file
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setCommand(String value) {#setCommand-java.lang.String-}
```
public void setCommand(String value)
```
Returns or sets the self defined command value text for the specified hyperlink.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setDiscardInput(boolean value) {#setDiscardInput-boolean-}
```
public void setDiscardInput(boolean value)
```
Indicates whether to discard user input at client browser when user click this CellCommand hyperlink. Could be used as an "undo" action.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setImageURL(String value) {#setImageURL-java.lang.String-}
```
public void setImageURL(String value)
```
Sets Image URL for the link, there is no imageurl properties in hyperlink, so actually use TextToDisplay to record this value ,TextToDisplay will be set to <img src=value > so it will change the value of TextToDisplay
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```
Returns or sets the ScreenTip text for the specified hyperlink.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTarget(String value) {#setTarget-java.lang.String-}
```
public void setTarget(String value)
```
Sets web link target type,please note this is an extension attribute and can not keep in excel file
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setTextToDisplay(String value) {#setTextToDisplay-java.lang.String-}
```
public void setTextToDisplay(String value)
```
Represents the text to be displayed for the specified hyperlink. The default value is the address of the hyperlink.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
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
