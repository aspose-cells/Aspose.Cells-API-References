##QueryTable
Represents QueryTable information.
**Inheritance:**
java.lang.Object
```
public class QueryTable
```
Represents QueryTable information.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
//Obtaining the reference of the first worksheet
Worksheet worksheet = workbook.getWorksheets().get(0);
//Getting the first query table in the worksheet if exists
//QueryTable qt = worksheet.QueryTables[0];
//Getting display address of the query table.
//string address = qt.ResultRange.Address;
```
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAdjustColumnWidth()](#getAdjustColumnWidth--) | Returns or sets the AdjustColumnWidth of the object. |
| [getClass()](#getClass--) |  |
| [getConnectionId()](#getConnectionId--) | Gets the connection id of the query table. |
| [getExternalConnection()](#getExternalConnection--) | Gets the relate external connection. |
| [getName()](#getName--) | Gets the name of querytable. |
| [getPreserveFormatting()](#getPreserveFormatting--) | Returns or sets the PreserveFormatting of the object. |
| [getResultRange()](#getResultRange--) | Gets the range of the result. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAdjustColumnWidth(boolean value)](#setAdjustColumnWidth-boolean-) | Returns or sets the AdjustColumnWidth of the object. |
| [setPreserveFormatting(boolean value)](#setPreserveFormatting-boolean-) | Returns or sets the PreserveFormatting of the object. |
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
### getAdjustColumnWidth() {#getAdjustColumnWidth--}
```
public boolean getAdjustColumnWidth()
```
Returns or sets the AdjustColumnWidth of the object.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getConnectionId() {#getConnectionId--}
```
public int getConnectionId()
```
Gets the connection id of the query table.
**Returns:**
int
### getExternalConnection() {#getExternalConnection--}
```
public ExternalConnection getExternalConnection()
```
Gets the relate external connection.
**Returns:**
[ExternalConnection](../../com.aspose.cells/externalconnection)
### getName() {#getName--}
```
public String getName()
```
Gets the name of querytable.
**Returns:**
java.lang.String
### getPreserveFormatting() {#getPreserveFormatting--}
```
public boolean getPreserveFormatting()
```
Returns or sets the PreserveFormatting of the object.
**Returns:**
boolean
### getResultRange() {#getResultRange--}
```
public Range getResultRange()
```
Gets the range of the result.
**Returns:**
[Range](../../com.aspose.cells/range) -
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
### setAdjustColumnWidth(boolean value) {#setAdjustColumnWidth-boolean-}
```
public void setAdjustColumnWidth(boolean value)
```
Returns or sets the AdjustColumnWidth of the object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPreserveFormatting(boolean value) {#setPreserveFormatting-boolean-}
```
public void setPreserveFormatting(boolean value)
```
Returns or sets the PreserveFormatting of the object.
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
