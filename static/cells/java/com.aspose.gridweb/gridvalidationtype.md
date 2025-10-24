##GridValidationType
Represents data validation type.
**Inheritance:**
java.lang.Object
```
public final class GridValidationType
```
Represents data validation type.
## Fields
| Field | Description |
| --- | --- |
| [ANY_VALUE](#ANY-VALUE) | Any value validation type. |
| [BOOLEAN](#BOOLEAN) | TRUE or FALSE |
| [CHECK_BOX](#CHECK-BOX) | Display the cell as a checkbox. |
| [CUSTOM](#CUSTOM) | Custom validation type. |
| [CUSTOM_EXPRESSION](#CUSTOM-EXPRESSION) | Custom validation type, using regular expression. |
| [CUSTOM_FUNCTION](#CUSTOM-FUNCTION) | Custom javascript function validation. |
| [CUSTOM_SERVER_FUNCTION](#CUSTOM-SERVER-FUNCTION) | Custom server-side function validation. |
| [DATE](#DATE) | Date validation type. |
| [DATE_TIME](#DATE-TIME) | DateTime (yyyy-MM-dd or yyyy-MM-dd hh:mm:ss). |
| [DECIMAL](#DECIMAL) | Decimal validation type. |
| [DROP_DOWN_LIST](#DROP-DOWN-LIST) | Show dropdown list. |
| [FREE_LIST](#FREE-LIST) | Free List validation type. |
| [LIST](#LIST) | List validation type. |
| [TEXT_LENGTH](#TEXT-LENGTH) | Text length validation type. |
| [TIME](#TIME) | Time validation type. |
| [WHOLE_NUMBER](#WHOLE-NUMBER) | Whole number validation type. |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ANY_VALUE {#ANY-VALUE}
```
public static final int ANY_VALUE
```
Any value validation type.
### BOOLEAN {#BOOLEAN}
```
public static final int BOOLEAN
```
TRUE or FALSE
### CHECK_BOX {#CHECK-BOX}
```
public static final int CHECK_BOX
```
Display the cell as a checkbox. And the value of the cell is True of False.
### CUSTOM {#CUSTOM}
```
public static final int CUSTOM
```
Custom validation type.
### CUSTOM_EXPRESSION {#CUSTOM-EXPRESSION}
```
public static final int CUSTOM_EXPRESSION
```
Custom validation type, using regular expression.
### CUSTOM_FUNCTION {#CUSTOM-FUNCTION}
```
public static final int CUSTOM_FUNCTION
```
Custom javascript function validation.
**Remarks**
Use the ClientValidationFunction property to specify the client validation function's name. The function should be declared as this formation:
function customValicationFunction(source, value)
The parameter "source" is the cell object. The parameter "value" is the string value of a cell to be checked. The function should returns true if the value is valid.
### CUSTOM_SERVER_FUNCTION {#CUSTOM-SERVER-FUNCTION}
```
public static final int CUSTOM_SERVER_FUNCTION
```
Custom server-side function validation.
**Remarks**
Use the CustomServerFunction property to specify the serverside validation . below is the example code:
first define class which implement GridCustomServerValidation class myservervali : GridCustomServerValidation
...... then add validation var gridValidationCollection = this.GridWeb.ActiveSheet.Validations;
GridValidation gv = gridValidationCollection.Add(new GridCellArea(1, 1, 2, 2));
gv.ValidationType = GridValidationType.CustomServerFunction; gv.ServerValidation = new myservervali(); then set ClientValidationFunction to deal with client logic when server validation fails and return message gv.ClientValidationFunction = "ValidationErrorClientFunction"; the client function shall be declared like this: function ValidationErrorClientFunction(cell,msg) please check demo page for a detail reference
### DATE {#DATE}
```
public static final int DATE
```
Date validation type.
### DATE_TIME {#DATE-TIME}
```
public static final int DATE_TIME
```
DateTime (yyyy-MM-dd or yyyy-MM-dd hh:mm:ss).
### DECIMAL {#DECIMAL}
```
public static final int DECIMAL
```
Decimal validation type.
### DROP_DOWN_LIST {#DROP-DOWN-LIST}
```
public static final int DROP_DOWN_LIST
```
Show dropdown list.
### FREE_LIST {#FREE-LIST}
```
public static final int FREE_LIST
```
Free List validation type.
### LIST {#LIST}
```
public static final int LIST
```
List validation type.
### TEXT_LENGTH {#TEXT-LENGTH}
```
public static final int TEXT_LENGTH
```
Text length validation type.
### TIME {#TIME}
```
public static final int TIME
```
Time validation type.
### WHOLE_NUMBER {#WHOLE-NUMBER}
```
public static final int WHOLE_NUMBER
```
Whole number validation type.
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
