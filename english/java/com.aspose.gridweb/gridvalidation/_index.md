---
title: GridValidation
second_title: Aspose.Cells for Java API Reference
description: Represents data validation.settings.
type: docs
url: /java/com.aspose.gridweb/gridvalidation/
---

**Inheritance:**
java.lang.Object
```
public class GridValidation
```

Represents data validation.settings.
## Constructors

| Constructor | Description |
| --- | --- |
| [GridValidation()](#GridValidation--) |  |
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
| [getClientValidationFunction()](#getClientValidationFunction--) | the client validation javascript function name. |
| [getErrorMessage()](#getErrorMessage--) | Represents the data validation error message. |
| [getErrorTitle()](#getErrorTitle--) | Represents the title of the data-validation error dialog box. |
| [getFormula1()](#getFormula1--) | Represents the value or expression associated with the data validation. |
| [getFormula2()](#getFormula2--) | Represents the value or expression associated with the second part of the data validation. |
| [getInputMessage()](#getInputMessage--) | Represents the data validation error message. |
| [getInputTitle()](#getInputTitle--) | Represents the title of the data-validation input dialog box. |
| [getListValue(int row, int column)](#getListValue-int-int-) | Get the value for list of the validation for the specified cell. |
| [getOperator()](#getOperator--) | Represents the operator for the data validation. |
| [getRegEx()](#getRegEx--) | the regular expression string. |
| [getShowError()](#getShowError--) | Indicates whether the data validation error message will be displayed whenever the user enters invalid data. |
| [getShowInput()](#getShowInput--) |  |
| [getValidationType()](#getValidationType--) | the validation type. |
| [getValue1()](#getValue1--) | Represents the value associated with the data validation. |
| [getValueList()](#getValueList--) | Gets/Sets the value list object. |
| [hashCode()](#hashCode--) |  |
| [isRequired()](#isRequired--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeACell(int row, int column)](#removeACell-int-int-) | Remove the validation settings in the cell. |
| [removeArea(GridCellArea cellArea)](#removeArea-com.aspose.gridweb.GridCellArea-) | Remove the validation settings in the range. |
| [setClientValidationFunction(String value)](#setClientValidationFunction-java.lang.String-) | For the description of this property, please see [getClientValidationFunction()](../../com.aspose.gridweb/gridvalidation\#getClientValidationFunction--) |
| [setErrorMessage(String value)](#setErrorMessage-java.lang.String-) | For the description of this property, please see [getErrorMessage()](../../com.aspose.gridweb/gridvalidation\#getErrorMessage--) |
| [setErrorTitle(String value)](#setErrorTitle-java.lang.String-) | For the description of this property, please see [getErrorTitle()](../../com.aspose.gridweb/gridvalidation\#getErrorTitle--) |
| [setFormula1(String value)](#setFormula1-java.lang.String-) | For the description of this property, please see [getFormula1()](../../com.aspose.gridweb/gridvalidation\#getFormula1--) |
| [setFormula2(String value)](#setFormula2-java.lang.String-) | For the description of this property, please see [getFormula2()](../../com.aspose.gridweb/gridvalidation\#getFormula2--) |
| [setInputMessage(String value)](#setInputMessage-java.lang.String-) | For the description of this property, please see [getInputMessage()](../../com.aspose.gridweb/gridvalidation\#getInputMessage--) |
| [setInputTitle(String value)](#setInputTitle-java.lang.String-) | For the description of this property, please see [getInputTitle()](../../com.aspose.gridweb/gridvalidation\#getInputTitle--) |
| [setOperator(int value)](#setOperator-int-) | For the description of this property, please see [getOperator()](../../com.aspose.gridweb/gridvalidation\#getOperator--) |
| [setRegEx(String value)](#setRegEx-java.lang.String-) | For the description of this property, please see [getRegEx()](../../com.aspose.gridweb/gridvalidation\#getRegEx--) |
| [setRequired(boolean value)](#setRequired-boolean-) | For the description of this property, please see [isRequired()](../../com.aspose.gridweb/gridvalidation\#isRequired--) |
| [setShowError(boolean value)](#setShowError-boolean-) | For the description of this property, please see [getShowError()](../../com.aspose.gridweb/gridvalidation\#getShowError--) |
| [setShowInput(boolean value)](#setShowInput-boolean-) | For the description of this property, please see [getShowInput()](../../com.aspose.gridweb/gridvalidation\#getShowInput--) |
| [setValidationType(int value)](#setValidationType-int-) | For the description of this property, please see [getValidationType()](../../com.aspose.gridweb/gridvalidation\#getValidationType--) |
| [setValueList(ArrayList<String> value)](#setValueList-java.util.ArrayList-java.lang.String--) | For the description of this property, please see [getValueList()](../../com.aspose.gridweb/gridvalidation\#getValueList--) |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### GridValidation() {#GridValidation--}
```
public GridValidation()
```


### ServerValidation {#ServerValidation}
```
public GridCustomServerValidation ServerValidation
```


Gets or sets the serverside validation javascript function name. Use the GridCustomServerValidation property to specify the serverside validation .

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


Applies the validation to the area. In this method , we will remove all old validations on this area.

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellArea | [GridCellArea](../../com.aspose.gridweb/gridcellarea) |  |

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


Represents a collection of [GridCellArea](../../com.aspose.gridweb/gridcellarea) which contains the data validation settings. The old valvidations on the area will not be removed if directly adding are to this list.

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


the client validation javascript function name. Use the ClientValidationFunction property to specify the client validation function's name. The function should be declared as this formation:
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


Get the value for list of the validation for the specified cell. Only for validation whose type is List and has been applied to given cell, otherwise null will be returned.

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

**Returns:**
int
### getRegEx() {#getRegEx--}
```
public String getRegEx()
```


the regular expression string.

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




**Returns:**
boolean
### getValidationType() {#getValidationType--}
```
public int getValidationType()
```


the validation type.

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


Gets/Sets the value list object.

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


For the description of this property, please see [getClientValidationFunction()](../../com.aspose.gridweb/gridvalidation\#getClientValidationFunction--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setErrorMessage(String value) {#setErrorMessage-java.lang.String-}
```
public void setErrorMessage(String value)
```


For the description of this property, please see [getErrorMessage()](../../com.aspose.gridweb/gridvalidation\#getErrorMessage--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setErrorTitle(String value) {#setErrorTitle-java.lang.String-}
```
public void setErrorTitle(String value)
```


For the description of this property, please see [getErrorTitle()](../../com.aspose.gridweb/gridvalidation\#getErrorTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFormula1(String value) {#setFormula1-java.lang.String-}
```
public void setFormula1(String value)
```


For the description of this property, please see [getFormula1()](../../com.aspose.gridweb/gridvalidation\#getFormula1--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setFormula2(String value) {#setFormula2-java.lang.String-}
```
public void setFormula2(String value)
```


For the description of this property, please see [getFormula2()](../../com.aspose.gridweb/gridvalidation\#getFormula2--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setInputMessage(String value) {#setInputMessage-java.lang.String-}
```
public void setInputMessage(String value)
```


For the description of this property, please see [getInputMessage()](../../com.aspose.gridweb/gridvalidation\#getInputMessage--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setInputTitle(String value) {#setInputTitle-java.lang.String-}
```
public void setInputTitle(String value)
```


For the description of this property, please see [getInputTitle()](../../com.aspose.gridweb/gridvalidation\#getInputTitle--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setOperator(int value) {#setOperator-int-}
```
public void setOperator(int value)
```


For the description of this property, please see [getOperator()](../../com.aspose.gridweb/gridvalidation\#getOperator--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setRegEx(String value) {#setRegEx-java.lang.String-}
```
public void setRegEx(String value)
```


For the description of this property, please see [getRegEx()](../../com.aspose.gridweb/gridvalidation\#getRegEx--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |

### setRequired(boolean value) {#setRequired-boolean-}
```
public void setRequired(boolean value)
```


For the description of this property, please see [isRequired()](../../com.aspose.gridweb/gridvalidation\#isRequired--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowError(boolean value) {#setShowError-boolean-}
```
public void setShowError(boolean value)
```


For the description of this property, please see [getShowError()](../../com.aspose.gridweb/gridvalidation\#getShowError--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setShowInput(boolean value) {#setShowInput-boolean-}
```
public void setShowInput(boolean value)
```


For the description of this property, please see [getShowInput()](../../com.aspose.gridweb/gridvalidation\#getShowInput--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |

### setValidationType(int value) {#setValidationType-int-}
```
public void setValidationType(int value)
```


For the description of this property, please see [getValidationType()](../../com.aspose.gridweb/gridvalidation\#getValidationType--)

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |

### setValueList(ArrayList<String> value) {#setValueList-java.util.ArrayList-java.lang.String--}
```
public void setValueList(ArrayList<String> value)
```


For the description of this property, please see [getValueList()](../../com.aspose.gridweb/gridvalidation\#getValueList--)

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

