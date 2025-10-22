##GridCell
Represents a cell object.
**Inheritance:**
java.lang.Object
```
public class GridCell
```
Represents a cell object.
## Methods
| Method | Description |
| --- | --- |
| [containsExternalLink()](#containsExternalLink--) | Indicates wether this cell contains an external link. |
| [copy(GridCell source)](#copy-com.aspose.gridweb.GridCell-) | Copies data from a source cell. |
| [copyStyle(GridTableItemStyle style)](#copyStyle-com.aspose.gridweb.GridTableItemStyle-) | copy the style and set the style for the cell |
| [createComment(String note, String author, boolean isvisible)](#createComment-java.lang.String-java.lang.String-boolean-) | Creates a comment object for a cell. |
| [createValidation(int validationType, boolean isRequried)](#createValidation-int-boolean-) | Creates a validation object for a cell. |
| [equals(Object obj)](#equals-java.lang.Object-) | Checks whether this object refers to the same cell with another cell object. |
| [getBoolValue()](#getBoolValue--) | Gets the boolean value contained in the cell. |
| [getClass()](#getClass--) |  |
| [getColumn()](#getColumn--) | Gets column number (zero based) of the cell. |
| [getComment()](#getComment--) | Get comment object on this cell |
| [getDateValue()](#getDateValue--) | Gets the DateTime value contained in the cell. |
| [getDisplayStringValue()](#getDisplayStringValue--) | Gets the formatted string value of this cell. |
| [getDoubleValue()](#getDoubleValue--) | Gets the double value contained in the cell. |
| [getFloatValue()](#getFloatValue--) | Gets the float value contained in the cell. |
| [getFormula()](#getFormula--) | Gets a formula of the [GridCell](../../com.aspose.gridweb/gridcell). |
| [getHtmlString()](#getHtmlString--) | Gets the html string which contains data and some formattings in this cell. |
| [getIntValue()](#getIntValue--) | Gets the integer value contained in the cell. |
| [getName()](#getName--) | Gets the name of the cell. |
| [getRow()](#getRow--) | Gets row number (zero based) of the cell. |
| [getStringValue()](#getStringValue--) | Gets the string value contained in the cell. |
| [getStyle()](#getStyle--) | Gets the copy of cell style. set the style for the cell. |
| [getType()](#getType--) | return the cell value type ,the meaning can see GridCellValueType.java |
| [getValue()](#getValue--) | Gets the value contained in this cell. |
| [getWidthOfValue()](#getWidthOfValue--) | Gets the width of the value in unit of pixels. |
| [hashCode()](#hashCode--) | Serves as a hash function for a particular type. |
| [isErrorValue()](#isErrorValue--) | Checks if a formula can properly evaluate a result. |
| [isFormula()](#isFormula--) | Represents if the specified cell contains formula. |
| [isStyleSet()](#isStyleSet--) | Indicates if the cell's style is set. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [putValue(boolean param_boolean)](#putValue-boolean-) | Puts a boolean value into the cell. |
| [putValue(DateTime param_date)](#putValue-com.aspose.gridweb.DateTime-) | Puts a DateTime value into the cell. |
| [putValue(double param_double)](#putValue-double-) | Puts a double value into the cell. |
| [putValue(int param_int)](#putValue-int-) | Puts a int value into the cell. |
| [putValue(Object objectValue)](#putValue-java.lang.Object-) | Puts an object value into the cell.same as setValue(Object param\_object) |
| [putValue(String param_string)](#putValue-java.lang.String-) | Puts a String value into the cell. |
| [putValue(String stringValue, boolean isConverted)](#putValue-java.lang.String-boolean-) | Puts a string value into the cell and converts the value to other data type if appropriate. |
| [putValue(String stringValue, boolean isConverted, boolean setStyle)](#putValue-java.lang.String-boolean-boolean-) | Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset. |
| [putValueAndSetFormatByValue(String stringValue)](#putValueAndSetFormatByValue-java.lang.String-) | Sets the cell's value with a string value and set cell format by this value. |
| [removeComment()](#removeComment--) | Removes the comment object of the cell. |
| [removeValidation()](#removeValidation--) | Removes the validation object of the cell. |
| [setBorder(WebBorderStyle borderStyle)](#setBorder-com.aspose.gridweb.WebBorderStyle-) | Sets borders(top,bottom,left and right) for a cell,all the borders have same borderstyle. |
| [setCustom(String custom)](#setCustom-java.lang.String-) | sets the custom format, null or empty string means no custom format. |
| [setFormula(String value)](#setFormula-java.lang.String-) | Sets a formula of the [GridCell](../../com.aspose.gridweb/gridcell). |
| [setFormula(String formula, Object value)](#setFormula-java.lang.String-java.lang.Object-) | Set the formula and the value of the formula. |
| [setHtmlString(String value)](#setHtmlString-java.lang.String-) | Sets the html string which contains data and some formattings in this cell. |
| [setNumberType(int numbertype)](#setNumberType-int-) | set the display format of numbers and dates |
| [setStyle(GridTableItemStyle value)](#setStyle-com.aspose.gridweb.GridTableItemStyle-) | Gets the copy of cell style. set the style for the cell. |
| [setValue(Object value)](#setValue-java.lang.Object-) | Gets the value contained in this cell. |
| [toString()](#toString--) | Returns a string represents the current Cell object. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### containsExternalLink() {#containsExternalLink--}
```
public boolean containsExternalLink()
```
Indicates wether this cell contains an external link. Only applies when the cell is a formula cell.
**Returns:**
boolean
### copy(GridCell source) {#copy-com.aspose.gridweb.GridCell-}
```
public void copy(GridCell source)
```
Copies data from a source cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [GridCell](../../com.aspose.gridweb/gridcell) | Source [GridCell](../../com.aspose.gridweb/gridcell) object. |
### copyStyle(GridTableItemStyle style) {#copyStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void copyStyle(GridTableItemStyle style)
```
copy the style and set the style for the cell
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| style | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) | The source style. |
### createComment(String note, String author, boolean isvisible) {#createComment-java.lang.String-java.lang.String-boolean-}
```
public GridComment createComment(String note, String author, boolean isvisible)
```
Creates a comment object for a cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| note | java.lang.String | comment note. |
| author | java.lang.String | comment author. |
| isvisible | boolean | whether the comment is visible. |
**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment) - GridComment object
### createValidation(int validationType, boolean isRequried) {#createValidation-int-boolean-}
```
public GridValidation createValidation(int validationType, boolean isRequried)
```
Creates a validation object for a cell.
**Example**
```
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.getActiveSheet();
GridValidation v = sheet.getCells().get("A1").createValidation(GridValidationType.CUSTOM_EXPRESSION, true);
// Sets to number validation expression.
v.setRegEx("\\d+");
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| validationType | int | [GridValidationType](../../com.aspose.gridweb/gridvalidationtype). Validation type. |
| isRequried | boolean | Whether the cell value is required. |
**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) -
### equals(Object obj) {#equals-java.lang.Object-}
```
public boolean equals(Object obj)
```
Checks whether this object refers to the same cell with another cell object.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| obj | java.lang.Object | another GridCell object |
**Returns:**
boolean - true if two cell objects refers to the same cell.
### getBoolValue() {#getBoolValue--}
```
public boolean getBoolValue()
```
Gets the boolean value contained in the cell.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getColumn() {#getColumn--}
```
public int getColumn()
```
Gets column number (zero based) of the cell.
**Returns:**
int
### getComment() {#getComment--}
```
public GridComment getComment()
```
Get comment object on this cell
**Returns:**
[GridComment](../../com.aspose.gridweb/gridcomment)
### getDateValue() {#getDateValue--}
```
public DateTime getDateValue()
```
Gets the DateTime value contained in the cell.
**Returns:**
[DateTime](../../com.aspose.gridweb/datetime)
### getDisplayStringValue() {#getDisplayStringValue--}
```
public String getDisplayStringValue()
```
Gets the formatted string value of this cell.
**Returns:**
java.lang.String
### getDoubleValue() {#getDoubleValue--}
```
public double getDoubleValue()
```
Gets the double value contained in the cell.
**Returns:**
double
### getFloatValue() {#getFloatValue--}
```
public float getFloatValue()
```
Gets the float value contained in the cell.
**Returns:**
float
### getFormula() {#getFormula--}
```
public String getFormula()
```
Gets a formula of the [GridCell](../../com.aspose.gridweb/gridcell).
**Remarks**
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimeter, such as "=SUM(A1, E1, H2)".
User can set any formula in Workbook designer file. Aspose.Cells will keep all the formulas. If user use this property to set a formula to a cell, major part of Workbook built-in functions is supported. And more is coming. If you have any special need for Workbook built-in functions, please let us know.
**Example**
```
GridWeb GridWeb1 = new GridWeb();
GridWorksheet sheet = GridWeb1.getActiveSheet();
sheet.getCells().get("B6").setFormula("=SUM(B2:B5, E1) + sheet1!A1");
```
**Returns:**
java.lang.String
### getHtmlString() {#getHtmlString--}
```
public String getHtmlString()
```
Gets the html string which contains data and some formattings in this cell.
**Returns:**
java.lang.String
### getIntValue() {#getIntValue--}
```
public int getIntValue()
```
Gets the integer value contained in the cell.
**Returns:**
int
### getName() {#getName--}
```
public String getName()
```
Gets the name of the cell. For example: A1, F102.
**Returns:**
java.lang.String
### getRow() {#getRow--}
```
public int getRow()
```
Gets row number (zero based) of the cell.
**Returns:**
int
### getStringValue() {#getStringValue--}
```
public String getStringValue()
```
Gets the string value contained in the cell.
**Returns:**
java.lang.String
### getStyle() {#getStyle--}
```
public GridTableItemStyle getStyle()
```
Gets the copy of cell style. set the style for the cell.
**Returns:**
[GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) - Style object.
### getType() {#getType--}
```
public int getType()
```
return the cell value type ,the meaning can see GridCellValueType.java
**Returns:**
int
### getValue() {#getValue--}
```
public Object getValue()
```
Gets the value contained in this cell.
**Remarks**
Possible type:
null,
Boolean,
DateTime,
Double,
Integer
String.
**Returns:**
java.lang.Object
### getWidthOfValue() {#getWidthOfValue--}
```
public int getWidthOfValue()
```
Gets the width of the value in unit of pixels.
**Returns:**
int -
### hashCode() {#hashCode--}
```
public int hashCode()
```
Serves as a hash function for a particular type.
**Returns:**
int - A hash code for current GridCell object.
### isErrorValue() {#isErrorValue--}
```
public boolean isErrorValue()
```
Checks if a formula can properly evaluate a result.
**Remarks**
Only applies to formula cell.
**Returns:**
boolean
### isFormula() {#isFormula--}
```
public boolean isFormula()
```
Represents if the specified cell contains formula.
**Returns:**
boolean
### isStyleSet() {#isStyleSet--}
```
public boolean isStyleSet()
```
Indicates if the cell's style is set. If return false, it means this cell has a default cell format.
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
### putValue(boolean param_boolean) {#putValue-boolean-}
```
public void putValue(boolean param_boolean)
```
Puts a boolean value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| param_boolean | boolean | Input value |
### putValue(DateTime param_date) {#putValue-com.aspose.gridweb.DateTime-}
```
public void putValue(DateTime param_date)
```
Puts a DateTime value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| param_date | [DateTime](../../com.aspose.gridweb/datetime) | Input value |
### putValue(double param_double) {#putValue-double-}
```
public void putValue(double param_double)
```
Puts a double value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| param_double | double | Input value |
### putValue(int param_int) {#putValue-int-}
```
public void putValue(int param_int)
```
Puts a int value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| param_int | int | Input value |
### putValue(Object objectValue) {#putValue-java.lang.Object-}
```
public void putValue(Object objectValue)
```
Puts an object value into the cell.same as setValue(Object param\_object)
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| objectValue | java.lang.Object | input value |
### putValue(String param_string) {#putValue-java.lang.String-}
```
public void putValue(String param_string)
```
Puts a String value into the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| param_string | java.lang.String | Input value |
### putValue(String stringValue, boolean isConverted) {#putValue-java.lang.String-boolean-}
```
public void putValue(String stringValue, boolean isConverted)
```
Puts a string value into the cell and converts the value to other data type if appropriate.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
### putValue(String stringValue, boolean isConverted, boolean setStyle) {#putValue-java.lang.String-boolean-boolean-}
```
public void putValue(String stringValue, boolean isConverted, boolean setStyle)
```
Puts a value into the cell, if appropriate the value will be converted to other data type and cell's number format will be reset.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Input value |
| isConverted | boolean | True: converted to other data type if appropriate. |
| setStyle | boolean | True: set the number format to cell's style when converting to other data type |
### putValueAndSetFormatByValue(String stringValue) {#putValueAndSetFormatByValue-java.lang.String-}
```
public void putValueAndSetFormatByValue(String stringValue)
```
Sets the cell's value with a string value and set cell format by this value.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| stringValue | java.lang.String | Input value. |
### removeComment() {#removeComment--}
```
public void removeComment()
```
Removes the comment object of the cell.
### removeValidation() {#removeValidation--}
```
public void removeValidation()
```
Removes the validation object of the cell.
### setBorder(WebBorderStyle borderStyle) {#setBorder-com.aspose.gridweb.WebBorderStyle-}
```
public void setBorder(WebBorderStyle borderStyle)
```
Sets borders(top,bottom,left and right) for a cell,all the borders have same borderstyle.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| borderStyle | [WebBorderStyle](../../com.aspose.gridweb/webborderstyle) | The border style. |
### setCustom(String custom) {#setCustom-java.lang.String-}
```
public void setCustom(String custom)
```
sets the custom format, null or empty string means no custom format.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| custom | java.lang.String | the custom string presentation |
### setFormula(String value) {#setFormula-java.lang.String-}
```
public void setFormula(String value)
```
Sets a formula of the [GridCell](../../com.aspose.gridweb/gridcell).
**Remarks**
A formula string always begins with an equal sign (=). And please always use comma(,) as parameters delimeter, such as "=SUM(A1, E1, H2)".
User can set any formula in Workbook designer file. Aspose.Cells will keep all the formulas. If user use this property to set a formula to a cell, major part of Workbook built-in functions is supported. And more is coming. If you have any special need for Workbook built-in functions, please let us know.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setFormula(String formula, Object value) {#setFormula-java.lang.String-java.lang.Object-}
```
public void setFormula(String formula, Object value)
```
Set the formula and the value of the formula.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| formula | java.lang.String | The formula. |
| value | java.lang.Object | The value of the formula. |
### setHtmlString(String value) {#setHtmlString-java.lang.String-}
```
public void setHtmlString(String value)
```
Sets the html string which contains data and some formattings in this cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### setNumberType(int numbertype) {#setNumberType-int-}
```
public void setNumberType(int numbertype)
```
set the display format of numbers and dates
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| numbertype | int | the value of ther numbertype,see GridTableItemStyle.NumberType |
### setStyle(GridTableItemStyle value) {#setStyle-com.aspose.gridweb.GridTableItemStyle-}
```
public void setStyle(GridTableItemStyle value)
```
Gets the copy of cell style. set the style for the cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [GridTableItemStyle](../../com.aspose.gridweb/gridtableitemstyle) |  |
### setValue(Object value) {#setValue-java.lang.Object-}
```
public void setValue(Object value)
```
Gets the value contained in this cell.
**Remarks**
Possible type:
null,
Boolean,
DateTime,
Double,
Integer
String.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.Object |  |
### toString() {#toString--}
```
public String toString()
```
Returns a string represents the current Cell object.
**Returns:**
java.lang.String -
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
