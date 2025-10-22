##ProtectedRange
A specified range to be allowed to edit when the sheet protection is ON.
**Inheritance:**
java.lang.Object
```
public class ProtectedRange
```
A specified range to be allowed to edit when the sheet protection is ON.
## Methods
| Method | Description |
| --- | --- |
| [addArea(int startRow, int startColumn, int endRow, int endColumn)](#addArea-int-int-int-int-) | Adds a referred area to this |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreas()](#getAreas--) | Gets all referred areas. |
| [getCellArea()](#getCellArea--) | Gets the [CellArea](../../com.aspose.cells/cellarea) object represents the cell area to be protected. |
| [getClass()](#getClass--) |  |
| [getName()](#getName--) | Gets the Range title. |
| [getPassword()](#getPassword--) | Represents the password to protect the range. |
| [getSecurityDescriptor()](#getSecurityDescriptor--) | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indicates whether the worksheets is protected with password. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setName(String value)](#setName-java.lang.String-) | Gets the Range title. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Represents the password to protect the range. |
| [setSecurityDescriptor(String value)](#setSecurityDescriptor-java.lang.String-) | The security descriptor defines user accounts who may edit this range without providing a password to access the range. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(int startRow, int startColumn, int endRow, int endColumn) {#addArea-int-int-int-int-}
```
public void addArea(int startRow, int startColumn, int endRow, int endColumn)
```
Adds a referred area to this
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| startRow | int | The start row. |
| startColumn | int | The start column. |
| endRow | int | The end row. |
| endColumn | int | The end column. |
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
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```
Gets all referred areas.
**Returns:**
com.aspose.cells.CellArea[] - Returns all referred areas.
### getCellArea() {#getCellArea--}
```
public CellArea getCellArea()
```
Gets the [CellArea](../../com.aspose.cells/cellarea) object represents the cell area to be protected.
**Returns:**
[CellArea](../../com.aspose.cells/cellarea)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getName() {#getName--}
```
public String getName()
```
Gets the Range title. This is used as a descriptor, not as a named range definition.
**Returns:**
java.lang.String
### getPassword() {#getPassword--}
```
public String getPassword()
```
Represents the password to protect the range.
**Returns:**
java.lang.String
### getSecurityDescriptor() {#getSecurityDescriptor--}
```
public String getSecurityDescriptor()
```
The security descriptor defines user accounts who may edit this range without providing a password to access the range.
**Returns:**
java.lang.String
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```
Indicates whether the worksheets is protected with password.
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
### setName(String value) {#setName-java.lang.String-}
```
public void setName(String value)
```
Gets the Range title. This is used as a descriptor, not as a named range definition.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```
Represents the password to protect the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setSecurityDescriptor(String value) {#setSecurityDescriptor-java.lang.String-}
```
public void setSecurityDescriptor(String value)
```
The security descriptor defines user accounts who may edit this range without providing a password to access the range.
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
