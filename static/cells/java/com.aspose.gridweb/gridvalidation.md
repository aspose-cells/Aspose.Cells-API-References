##GridValidation
Represents data validation.settings.
**Inheritance:**
java.lang.Object
```
public class GridValidation
```
Represents data validation.settings.
## Fields
| Field | Description |
| --- | --- |
| [ServerValidation](#ServerValidation) | Gets or sets the serverside validation javascript function name. |
## Methods
| Method | Description |
| --- | --- |
| [addACell(int row, int column)](#addACell-int-int-) | add the validation settings in the cell. |
| [addACell(String cellname)](#addACell-java.lang.String-) | add the validation settings in the cell. |
| [addArea(GridCellArea cellArea)](#addArea-com.aspose.gridweb.GridCellArea-) | Applies the validation to the area. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAreaList()](#getAreaList--) | Represents a collection of [GridCellArea](../../com.aspose.gridweb/gridcellarea) which contains the data validation settings. |
| [getClass()](#getClass--) |  |
| [getClientValidationFunction()](#getClientValidationFunction--) | Gets the client validation javascript function name. |
| [getErrorMessage()](#getErrorMessage--) | Represents the data validation error message. |
| [getErrorTitle()](#getErrorTitle--) | Represents the title of the data-validation error dialog box. |
| [getFormula1()](#getFormula1--) | Represents the value or expression associated with the data validation. |
| [getFormula2()](#getFormula2--) | Represents the value or expression associated with the second part of the data validation. |
| [getInputMessage()](#getInputMessage--) | Represents the data validation error message. |
| [getInputTitle()](#getInputTitle--) | Represents the title of the data-validation input dialog box. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Get the value for list of the validation for the specified cell. |
| [getOperator()](#getOperator--) | Represents the operator for the data validation. |
| [getRegEx()](#getRegEx--) | Gets the regular expression string. |
| [getShowError()](#getShowError--) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [getShowInput()](#getShowInput--) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [getValidationType()](#getValidationType--) | Gets the validation type. |
| [getValue1()](#getValue1--) | Represents the value associated with the data validation. |
| [getValueList()](#getValueList--) | Gets the value list object. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) | Gets whether the cell value is required. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Remove the validation settings in the cell. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Remove the validation settings in the range. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | Sets the client validation javascript function name. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Represents the data validation error message. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Represents the title of the data-validation error dialog box. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Represents the value or expression associated with the data validation. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Represents the value or expression associated with the second part of the data validation. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Represents the data validation error message. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Represents the title of the data-validation input dialog box. |
| [setOperator(int value)](#setOperator-int-) | Represents the operator for the data validation. |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | Sets the regular expression string. |
| [setRequired(boolean value)](#setRequired-boolean-) | Sets whether the cell value is required. |
| [setShowError(boolean value)](#setShowError-boolean-) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [setValidationType(int value)](#setValidationType-int-) | Sets the validation type. |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | Sets the value list object. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```
Gets or sets the serverside validation javascript function name.
**Remarks**
Use the GridCustomServerValidation property to specify the serverside validation .
### addACell(int row, int column) {#addACell-int-int-}
```
public void addACell(int row, int column)
```
add the validation settings in the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |
### addACell(String cellname) {#addACell-java.lang.String-}
```
public void addACell(String cellname)
```
add the validation settings in the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellname | java.lang.String | cell name. |
### addArea(GridCellArea cellArea) {#addArea-com.aspose.gridweb.GridCellArea-}
```
public void addArea(GridCellArea cellArea)
```
Applies the validation to the area.
**Remarks**
In this method , we will remove all old validations on this area.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | The area. |
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
### getAreaList() {#getAreaList--}
```
public ArrayList getAreaList()
```
Represents a collection of [GridCellArea](../../com.aspose.gridweb/gridcellarea) which contains the data validation settings.
**Remarks**
The old valvidations on the area will not be removed if directly adding are to this list.
**Returns:**
java.util.ArrayList
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getClientValidationFunction() {#getClientValidationFunction--}
```
public String getClientValidationFunction()
```
Gets the client validation javascript function name.
**Remarks**
Use the ClientValidationFunction property to specify the client validation function's name. The function should be declared as this formation:
function customValicationFunction(source, value)
The parameter "source" is the cell object. The parameter "value" is the string value of a cell to be checked. The function should returns true if the value is valid.
**Returns:**
java.lang.String
### getErrorMessage() {#getErrorMessage--}
```
public String getErrorMessage()
```
Represents the data validation error message.
**Returns:**
java.lang.String
### getErrorTitle() {#getErrorTitle--}
```
public String getErrorTitle()
```
Represents the title of the data-validation error dialog box.
**Returns:**
java.lang.String
### getFormula1() {#getFormula1--}
```
public String getFormula1()
```
Represents the value or expression associated with the data validation.
**Returns:**
java.lang.String
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```
Represents the value or expression associated with the second part of the data validation.
**Returns:**
java.lang.String
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```
Represents the data validation error message.
**Returns:**
java.lang.String
### getInputTitle() {#getInputTitle--}
```
public String getInputTitle()
```
Represents the title of the data-validation input dialog box.
**Returns:**
java.lang.String
### getListValue(int row, int column) {#getListValue-int-int-}
```
public Object getListValue(int row, int column)
```
Get the value for list of the validation for the specified cell.
**Remarks**
Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |
**Returns:**
java.lang.Object - The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a ReferredArea object; Otherwise the returned value may be null, object[], or simple object.
### getOperator() {#getOperator--}
```
public int getOperator()
```
Represents the operator for the data validation.
See [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).
**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```
Gets the regular expression string.
**Returns:**
java.lang.String
### getShowError() {#getShowError--}
```
public boolean getShowError()
```
Indicates whether the data validation error message will be displayed whenever the user enters invalid data.
**Returns:**
boolean
### getShowInput() {#getShowInput--}
```
public boolean getShowInput()
```
Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.
**Returns:**
boolean
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```
Gets the validation type.
See [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).
**Returns:**
int
### getValue1() {#getValue1--}
```
public Object[] getValue1()
```
Represents the value associated with the data validation.
**Returns:**
java.lang.Object[]
### getValueList() {#getValueList--}
```
public ArrayList<String> getValueList()
```
Gets the value list object.
**Returns:**
java.util.ArrayList<java.lang.String>
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isRequired() {#isRequired--}
```
public boolean isRequired()
```
Gets whether the cell value is required.
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
### removeACell(int row, int column) {#removeACell-int-int-}
```
public void removeACell(int row, int column)
```
Remove the validation settings in the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |
### removeArea(GridCellArea cellArea) {#removeArea-com.aspose.gridweb.GridCellArea-}
```
public void removeArea(GridCellArea cellArea)
```
Remove the validation settings in the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | The range which contains the data validation settings. |
### setClientValidationFunction(String value) {#setClientValidationFunction-java.lang.String-}
```
public void setClientValidationFunction(String value)
```
Sets the client validation javascript function name.
**Remarks**
Use the ClientValidationFunction property to specify the client validation function's name. The function should be declared as this formation:
function customValicationFunction(source, value)
The parameter "source" is the cell object. The parameter "value" is the string value of a cell to be checked. The function should returns true if the value is valid.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```
Represents the data validation error message.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```
Represents the title of the data-validation error dialog box.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```
Represents the value or expression associated with the data validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```
Represents the value or expression associated with the second part of the data validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```
Represents the data validation error message.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```
Represents the title of the data-validation input dialog box.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```
Represents the operator for the data validation.
See [GridOperatorType](../../com.aspose.gridweb/gridoperatortype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```
Sets the regular expression string.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```
Sets whether the cell value is required.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```
Indicates whether the data validation error message will be displayed whenever the user enters invalid data.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```
Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```
Sets the validation type.
See [GridValidationType](../../com.aspose.gridweb/gridvalidationtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```
Sets the value list object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.util.ArrayList<java.lang.String> |  |
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
