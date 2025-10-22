##Hyperlink
Encapsulates the object that represents a hyperlink.
**Inheritance:**
java.lang.Object
```
public class Hyperlink
```
Encapsulates the object that represents a hyperlink.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Adding a new worksheet to the Workbook object
workbook.getWorksheets().add();
//Obtaining the reference of the newly added worksheet by passing its sheet index
Worksheet worksheet = workbook.getWorksheets().get(0);
//Adding a hyperlink to a URL at "A1" cell
int index = worksheet.getHyperlinks().add("A1", 1, 1, "http://www.aspose.com");
//Getting a Hyperlink by index.
Hyperlink hyperlink = worksheet.getHyperlinks().get(index);
//Setting display text of this hyperlink.
hyperlink.setTextToDisplay("Aspose");
//Saving the Excel file
workbook.save("book1.xls");
```
## Methods
| Method | Description |
| --- | --- |
| [delete()](#delete--) | Deletes this hyperlink |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAddress()](#getAddress--) | Represents the address of a hyperlink. |
| [getArea()](#getArea--) | Gets the range of hyperlink. |
| [getClass()](#getClass--) |  |
| [getLinkType()](#getLinkType--) | Gets the link type. |
| [getScreenTip()](#getScreenTip--) | Returns or sets the ScreenTip text for the specified hyperlink. |
| [getTextToDisplay()](#getTextToDisplay--) | Represents the text to be displayed for the specified hyperlink. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAddress(String value)](#setAddress-java.lang.String-) | Represents the address of a hyperlink. |
| [setScreenTip(String value)](#setScreenTip-java.lang.String-) | Returns or sets the ScreenTip text for the specified hyperlink. |
| [setTextToDisplay(String value)](#setTextToDisplay-java.lang.String-) | Represents the text to be displayed for the specified hyperlink. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### delete() {#delete--}
```
public void delete()
```
Deletes this hyperlink
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
### getArea() {#getArea--}
```
public CellArea getArea()
```
Gets the range of hyperlink.
**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getLinkType() {#getLinkType--}
```
public int getLinkType()
```
Gets the link type.
See [TargetModeType](../../com.aspose.cells/targetmodetype).
**Returns:**
int
### getScreenTip() {#getScreenTip--}
```
public String getScreenTip()
```
Returns or sets the ScreenTip text for the specified hyperlink.
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
### setScreenTip(String value) {#setScreenTip-java.lang.String-}
```
public void setScreenTip(String value)
```
Returns or sets the ScreenTip text for the specified hyperlink.
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
