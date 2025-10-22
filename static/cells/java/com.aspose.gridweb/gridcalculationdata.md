##GridCalculationData
Represents the required data when calculating one function such as function name parameters ...etc.
**Inheritance:**
java.lang.Object
```
public class GridCalculationData
```
Represents the required data when calculating one function, such as function name, parameters, ...etc.
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getCalculatedValue()](#getCalculatedValue--) | Gets the calculated value for this function. |
| [getCell()](#getCell--) | Gets the Cell object where the function is in. |
| [getClass()](#getClass--) |  |
| [getFunctionName()](#getFunctionName--) | Gets the function name to be calculated. |
| [getParamCount()](#getParamCount--) | Gets the count of parameters |
| [getParamText(int index)](#getParamText-int-) | Gets the literal text of the parameter at given index. |
| [getParamValue(int index)](#getParamValue-int-) | Gets the represented value object of the parameter at given index. |
| [getWorkbook()](#getWorkbook--) | Gets the Workbook object where the function is in. |
| [getWorksheet()](#getWorksheet--) | Gets the Workbook object where the function is in. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setCalculatedValue(Object value)](#setCalculatedValue-java.lang.Object-) | Sets the calculated value for this function. |
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
### getCalculatedValue() {#getCalculatedValue--}
```
public Object getCalculatedValue()
```
Gets the calculated value for this function.
**Remarks**
User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property. Getting this property before setting will make the function be calculated by the default calculation engine of Aspose.Cells and the calculated value will be returned.
**Returns:**
java.lang.Object
### getCell() {#getCell--}
```
public GridCell getCell()
```
Gets the Cell object where the function is in.
**Returns:**
[GridCell](../../com.aspose.gridweb/gridcell)
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getFunctionName() {#getFunctionName--}
```
public String getFunctionName()
```
Gets the function name to be calculated.
**Returns:**
java.lang.String
### getParamCount() {#getParamCount--}
```
public int getParamCount()
```
Gets the count of parameters
**Returns:**
int
### getParamText(int index) {#getParamText-int-}
```
public String getParamText(int index)
```
Gets the literal text of the parameter at given index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | index of the parameter(0 based) |
**Returns:**
java.lang.String - literal text of the parameter
### getParamValue(int index) {#getParamValue-int-}
```
public Object getParamValue(int index)
```
Gets the represented value object of the parameter at given index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | index of the parameter(0 based) |
**Returns:**
java.lang.Object - If the parameter is plain value, then returns the plain value. If the parameter is reference, then return ReferredArea object.
### getWorkbook() {#getWorkbook--}
```
public GridWorkbook getWorkbook()
```
Gets the Workbook object where the function is in.
**Returns:**
[GridWorkbook](../../com.aspose.gridweb/gridworkbook)
### getWorksheet() {#getWorksheet--}
```
public GridWorksheet getWorksheet()
```
Gets the Workbook object where the function is in.
**Returns:**
[GridWorksheet](../../com.aspose.gridweb/gridworksheet)
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
### setCalculatedValue(Object value) {#setCalculatedValue-java.lang.Object-}
```
public void setCalculatedValue(Object value)
```
Sets the calculated value for this function.
**Remarks**
User should set this property in his custom calculation engine for those functions the engine supports, and the set value will be returned when getting this property. Getting this property before setting will make the function be calculated by the default calculation engine of Aspose.Cells and the calculated value will be returned.
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
