##Validation
Represents data validation.settings.
**Inheritance:**
java.lang.Object
```
public class Validation
```
Represents data validation.settings.
**Example**
```
Workbook workbook = new Workbook();
ValidationCollection validations = workbook.getWorksheets().get(0).getValidations();
CellArea area = CellArea.createCellArea(0, 0, 1, 1);
Validation validation = validations.get(validations.add(area));
validation.setType(com.aspose.cells.ValidationType.WHOLE_NUMBER);
validation.setOperator(OperatorType.BETWEEN);
validation.setFormula1("3");
validation.setFormula2("1234");
```
## Methods
| Method | Description |
| --- | --- |
| [addArea(CellArea cellArea)](#addArea-com.aspose.cells.CellArea-) | Applies the validation to the area. |
| [addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)](#addArea-com.aspose.cells.CellArea-boolean-boolean-) | Applies the validation to the area. |
| [addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)](#addAreas-com.aspose.cells.CellArea---boolean-boolean-) | Applies the validation to given areas. |
| [copy(Validation source, CopyOptions copyOption)](#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-) | Copy validation. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAlertStyle()](#getAlertStyle--) | Represents the validation alert style. |
| [getAreas()](#getAreas--) | Gets all [CellArea](../../com.aspose.cells/cellarea) which contain the data validation settings. |
| [getClass()](#getClass--) |  |
| [getErrorMessage()](#getErrorMessage--) | Represents the data validation error message. |
| [getErrorTitle()](#getErrorTitle--) | Represents the title of the data-validation error dialog box. |
| [getFormula1()](#getFormula1--) | Represents the value or expression associated with the data validation. |
| [getFormula1(boolean isR1C1, boolean isLocal)](#getFormula1-boolean-boolean-) | Gets the value or expression associated with this validation. |
| [getFormula1(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula1-boolean-boolean-int-int-) | Gets the value or expression associated with this validation for specific cell. |
| [getFormula2()](#getFormula2--) | Represents the value or expression associated with the data validation. |
| [getFormula2(boolean isR1C1, boolean isLocal)](#getFormula2-boolean-boolean-) | Gets the value or expression associated with this validation. |
| [getFormula2(boolean isR1C1, boolean isLocal, int row, int column)](#getFormula2-boolean-boolean-int-int-) | Gets the value or expression associated with this validation for specific cell. |
| [getIgnoreBlank()](#getIgnoreBlank--) | Indicates whether blank values are permitted by the range data validation. |
| [getInCellDropDown()](#getInCellDropDown--) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [getInputMessage()](#getInputMessage--) | Represents the data validation input message. |
| [getInputTitle()](#getInputTitle--) | Represents the title of the data-validation input dialog box. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Get the value for list of the validation for the specified cell. |
| [getOperator()](#getOperator--) | Represents the operator for the data validation. |
| [getShowError()](#getShowError--) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [getShowInput()](#getShowInput--) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [getType()](#getType--) | Represents the data validation type. |
| [getValue(int row, int column, boolean isValue1)](#getValue-int-int-boolean-) | Get the value of validation on the specific cell. |
| [getValue1()](#getValue1--) | Represents the first value associated with the data validation. |
| [getValue2()](#getValue2--) | Represents the second value associated with the data validation. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Remove the validation settings in the cell. |
| [removeArea(CellArea cellArea)](#removeArea-com.aspose.cells.CellArea-) | Remove the validation settings in the range. |
| [removeAreas(CellArea[] areas)](#removeAreas-com.aspose.cells.CellArea---) | Removes this validation from given areas. |
| [setAlertStyle(int value)](#setAlertStyle-int-) | Represents the validation alert style. |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | Represents the data validation error message. |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | Represents the title of the data-validation error dialog box. |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | Represents the value or expression associated with the data validation. |
| [setFormula1(String formula, boolean isR1C1, boolean isLocal)](#setFormula1-java.lang.String-boolean-boolean-) | Sets the value or expression associated with this validation. |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | Represents the value or expression associated with the data validation. |
| [setFormula2(String formula, boolean isR1C1, boolean isLocal)](#setFormula2-java.lang.String-boolean-boolean-) | Sets the value or expression associated with this validation. |
| [setIgnoreBlank(boolean value)](#setIgnoreBlank-boolean-) | Indicates whether blank values are permitted by the range data validation. |
| [setInCellDropDown(boolean value)](#setInCellDropDown-boolean-) | Indicates whether data validation displays a drop-down list that contains acceptable values. |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | Represents the data validation input message. |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | Represents the title of the data-validation input dialog box. |
| [setOperator(int value)](#setOperator-int-) | Represents the operator for the data validation. |
| [setShowError(boolean value)](#setShowError-boolean-) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [setShowInput(boolean value)](#setShowInput-boolean-) | Indicates whether the data validation input message will be displayed whenever the user selects a cell in the data validation range. |
| [setType(int value)](#setType-int-) | Represents the data validation type. |
| [setValue1(Object value)](#setValue1-java.lang.Object-) | Represents the first value associated with the data validation. |
| [setValue2(Object value)](#setValue2-java.lang.Object-) | Represents the second value associated with the data validation. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addArea(CellArea cellArea) {#addArea-com.aspose.cells.CellArea-}
```
public void addArea(CellArea cellArea)
```
Applies the validation to the area.
**Remarks**
It is equivalent to use [addArea(CellArea,boolean,boolean)](../../com.aspose.cells/validation\#addArea-CellArea-boolean-boolean-) with checking intersection and edge.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | The area. |
### addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge) {#addArea-com.aspose.cells.CellArea-boolean-boolean-}
```
public void addArea(CellArea cellArea, boolean checkIntersection, boolean checkEdge)
```
Applies the validation to the area.
**Remarks**
In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | The area. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that the added area does not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if given area will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that the added area is not the top-left one, this parameter can be set as false for performance consideration. |
### addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge) {#addAreas-com.aspose.cells.CellArea---boolean-boolean-}
```
public void addAreas(CellArea[] areas, boolean checkIntersection, boolean checkEdge)
```
Applies the validation to given areas.
**Remarks**
In this method, we will remove all old validations in given area. For the top-left one of Validation's applied ranges, firstly its StartRow is smallest, secondly its StartColumn is the smallest one of those areas who have the same smallest StartRow.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | The areas. |
| checkIntersection | boolean | Whether check the intersection of given area with existing validations' areas. If one validation has been applied in given area(or part of it), then the existing validation should be removed at first from given area. Otherwise corruption may be caused for the generated Validations. If user is sure that all the added areas do not intersect with any existing area, this parameter can be set as false for performance consideration. |
| checkEdge | boolean | Whether check the edge of this validation's applied areas. Validation's internal settings depend on the top-left one of its applied ranges, so if one of given areas will become the new top-left one of the applied ranges, the internal settings should be changed and rebuilt, otherwise unexpected result may be caused. If user is sure that no one of those added areas is the top-left, this parameter can be set as false for performance consideration. |
### copy(Validation source, CopyOptions copyOption) {#copy-com.aspose.cells.Validation-com.aspose.cells.CopyOptions-}
```
public void copy(Validation source, CopyOptions copyOption)
```
Copy validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Validation](../../com.aspose.cells/validation) | The source validation. |
| copyOption | [CopyOptions](../../com.aspose.cells/copyoptions) | The copy option. |
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
### getAlertStyle() {#getAlertStyle--}
```
public int getAlertStyle()
```
Represents the validation alert style.
See [ValidationAlertType](../../com.aspose.cells/validationalerttype).
**Returns:**
int
### getAreas() {#getAreas--}
```
public CellArea[] getAreas()
```
Gets all [CellArea](../../com.aspose.cells/cellarea) which contain the data validation settings.
**Returns:**
com.aspose.cells.CellArea[]
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
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
### getFormula1(boolean isR1C1, boolean isLocal) {#getFormula1-boolean-boolean-}
```
public String getFormula1(boolean isR1C1, boolean isLocal)
```
Gets the value or expression associated with this validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns:**
java.lang.String - The value or expression associated with this validation.
### getFormula1(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula1-boolean-boolean-int-int-}
```
public String getFormula1(boolean isR1C1, boolean isLocal, int row, int column)
```
Gets the value or expression associated with this validation for specific cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | int | The row index. |
| column | int | The column index. |
**Returns:**
java.lang.String - The value or expression associated with this validation.
### getFormula2() {#getFormula2--}
```
public String getFormula2()
```
Represents the value or expression associated with the data validation.
**Returns:**
java.lang.String
### getFormula2(boolean isR1C1, boolean isLocal) {#getFormula2-boolean-boolean-}
```
public String getFormula2(boolean isR1C1, boolean isLocal)
```
Gets the value or expression associated with this validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
**Returns:**
java.lang.String - The value or expression associated with this validation.
### getFormula2(boolean isR1C1, boolean isLocal, int row, int column) {#getFormula2-boolean-boolean-int-int-}
```
public String getFormula2(boolean isR1C1, boolean isLocal, int row, int column)
```
Gets the value or expression associated with this validation for specific cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| isR1C1 | boolean | Whether the formula needs to be formatted as R1C1. |
| isLocal | boolean | Whether the formula needs to be formatted by locale. |
| row | int | The row index. |
| column | int | The column index. |
**Returns:**
java.lang.String - The value or expression associated with this validation.
### getIgnoreBlank() {#getIgnoreBlank--}
```
public boolean getIgnoreBlank()
```
Indicates whether blank values are permitted by the range data validation.
**Returns:**
boolean
### getInCellDropDown() {#getInCellDropDown--}
```
public boolean getInCellDropDown()
```
Indicates whether data validation displays a drop-down list that contains acceptable values.
**Returns:**
boolean
### getInputMessage() {#getInputMessage--}
```
public String getInputMessage()
```
Represents the data validation input message.
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
java.lang.Object - The value to produce the list of this validation for the specified cell. If the list references to a range, then the returned value will be a [ReferredArea](../../com.aspose.cells/referredarea) object; Otherwise the returned value may be null, object[], or simple object.
### getOperator() {#getOperator--}
```
public int getOperator()
```
Represents the operator for the data validation.
See [OperatorType](../../com.aspose.cells/operatortype).
**Returns:**
int
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
### getType() {#getType--}
```
public int getType()
```
Represents the data validation type.
See [ValidationType](../../com.aspose.cells/validationtype).
**Returns:**
int
### getValue(int row, int column, boolean isValue1) {#getValue-int-int-boolean-}
```
public Object getValue(int row, int column, boolean isValue1)
```
Get the value of validation on the specific cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |
| isValue1 | boolean | Indicates whether getting the first value. |
**Returns:**
java.lang.Object -
### getValue1() {#getValue1--}
```
public Object getValue1()
```
Represents the first value associated with the data validation.
**Returns:**
java.lang.Object
### getValue2() {#getValue2--}
```
public Object getValue2()
```
Represents the second value associated with the data validation.
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
### removeArea(CellArea cellArea) {#removeArea-com.aspose.cells.CellArea-}
```
public void removeArea(CellArea cellArea)
```
Remove the validation settings in the range.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [CellArea](../../com.aspose.cells/cellarea) | the areas where this validation settings should be removed. |
### removeAreas(CellArea[] areas) {#removeAreas-com.aspose.cells.CellArea---}
```
public void removeAreas(CellArea[] areas)
```
Removes this validation from given areas.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| areas | [CellArea\[\]](../../com.aspose.cells/cellarea) | the areas where this validation settings should be removed. |
### setAlertStyle(int value) {#setAlertStyle-int-}
```
public void setAlertStyle(int value)
```
Represents the validation alert style.
See [ValidationAlertType](../../com.aspose.cells/validationalerttype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
### setFormula1(String formula, boolean isR1C1, boolean isLocal) {#setFormula1-java.lang.String-boolean-boolean-}
```
public void setFormula1(String formula, boolean isR1C1, boolean isLocal)
```
Sets the value or expression associated with this validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The value or expression associated with this format condition. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```
Represents the value or expression associated with the data validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFormula2(String formula, boolean isR1C1, boolean isLocal) {#setFormula2-java.lang.String-boolean-boolean-}
```
public void setFormula2(String formula, boolean isR1C1, boolean isLocal)
```
Sets the value or expression associated with this validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The value or expression associated with this format condition. |
| isR1C1 | boolean | Whether the formula is R1C1 formula. |
| isLocal | boolean | Whether the formula is locale formatted. |
### setIgnoreBlank(boolean value) {#setIgnoreBlank-boolean-}
```
public void setIgnoreBlank(boolean value)
```
Indicates whether blank values are permitted by the range data validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setInCellDropDown(boolean value) {#setInCellDropDown-boolean-}
```
public void setInCellDropDown(boolean value)
```
Indicates whether data validation displays a drop-down list that contains acceptable values.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```
Represents the data validation input message.
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
See [OperatorType](../../com.aspose.cells/operatortype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
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
### setType(int value) {#setType-int-}
```
public void setType(int value)
```
Represents the data validation type.
See [ValidationType](../../com.aspose.cells/validationtype).
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setValue1(Object value) {#setValue1-java.lang.Object-}
```
public void setValue1(Object value)
```
Represents the first value associated with the data validation.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
### setValue2(Object value) {#setValue2-java.lang.Object-}
```
public void setValue2(Object value)
```
Represents the second value associated with the data validation.
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
