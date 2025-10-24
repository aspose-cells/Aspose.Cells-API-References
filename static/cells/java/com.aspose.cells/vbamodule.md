##VbaModule
Represents the module in VBA project.
**Inheritance:**
java.lang.Object
```
public class VbaModule
```
Represents the module in VBA project.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
// Init VBA project.
VbaProject vbaProject = workbook.getVbaProject();
// Add a new module.
int index = vbaProject.getModules().add(VbaModuleType.CLASS, "test");
// Get vba module
VbaModule vbaModule = vbaProject.getModules().get(index);
// Set codes
vbaModule.setCodes("Sub ShowMessage()\r\nMsgBox \"Welcome to Aspose!\"\r\nEnd Sub");
//Saving the Excel file
workbook.save("book1.xlsm");
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getBinaryCodes()](#getBinaryCodes--) | Gets the binary codes of module. |
| [getClass()](#getClass--) |  |
| [getCodes()](#getCodes--) | Gets the codes of module. |
| [getName()](#getName--) | Gets the name of Module. |
| [getType()](#getType--) | Gets the type of module. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCodes(String value)](#setCodes-java.lang.String-) | Sets the codes of module. |
| [setName(String value)](#setName-java.lang.String-) | Sets the name of Module. |
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
### getBinaryCodes() {#getBinaryCodes--}
```
public byte[] getBinaryCodes()
```
Gets the binary codes of module.
**Returns:**
byte[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCodes() {#getCodes--}
```
public String getCodes()
```
Gets the codes of module.
**Returns:**
java.lang.String
### getName() {#getName--}
```
public String getName()
```
Gets the name of Module.
**Returns:**
java.lang.String
### getType() {#getType--}
```
public int getType()
```
Gets the type of module.
See [VbaModuleType](../../com.aspose.cells/vbamoduletype).
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
### setCodes(String value) {#setCodes-java.lang.String-}
```
public void setCodes(String value)
```
Sets the codes of module.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Sets the name of Module.
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
