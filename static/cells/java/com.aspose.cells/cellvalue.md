##CellValue
Represents the cell value and corresponding type.
**Inheritance:**
java.lang.Object
```
public class CellValue
```
Represents the cell value and corresponding type.
## Constructors
| Constructor | Description |
| --- | --- |
| [CellValue()](#CellValue--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getType()](#getType--) | Gets the type of cell value. |
| [getValue()](#getValue--) | Gets the cell value. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setType(int value)](#setType-int-) | Sets the type of cell value. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Sets the cell value. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### CellValue() {#CellValue--}
```
public CellValue()
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
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getType() {#getType--}
```
public int getType()
```
Gets the type of cell value.
See [CellValueType](../../com.aspose.cells/cellvaluetype).
**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```
Gets the cell value.
**Remarks**
The value must be of the correct type of object corresponding to the [getType()](../../com.aspose.cells/cellvalue\#getType--):
| Type                                                                              | Value                                           |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL)            | null, any other object will be ignored          |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC)      | double                                          |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime                                        |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING)        | string                                          |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL)            | bool                                            |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR)          | error string such as "\#VALUE!", "\#NAME?", ... |
**Returns:**
java.lang.Object
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
### setType(int value) {#setType-int-}
```
public void setType(int value)
```
Sets the type of cell value.
See [CellValueType](../../com.aspose.cells/cellvaluetype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```
Sets the cell value.
**Remarks**
The value must be of the correct type of object corresponding to the [getType()](../../com.aspose.cells/cellvalue\#getType--):
| Type                                                                              | Value                                           |
| --------------------------------------------------------------------------------- | ----------------------------------------------- |
| [CellValueType.IS\_NULL](../../com.aspose.cells/cellvaluetype\#IS-NULL)            | null, any other object will be ignored          |
| [CellValueType.IS\_NUMERIC](../../com.aspose.cells/cellvaluetype\#IS-NUMERIC)      | double                                          |
| [CellValueType.IS\_DATE\_TIME](../../com.aspose.cells/cellvaluetype\#IS-DATE-TIME) | DateTime                                        |
| [CellValueType.IS\_STRING](../../com.aspose.cells/cellvaluetype\#IS-STRING)        | string                                          |
| [CellValueType.IS\_BOOL](../../com.aspose.cells/cellvaluetype\#IS-BOOL)            | bool                                            |
| [CellValueType.IS\_ERROR](../../com.aspose.cells/cellvaluetype\#IS-ERROR)          | error string such as "\#VALUE!", "\#NAME?", ... |
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
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
