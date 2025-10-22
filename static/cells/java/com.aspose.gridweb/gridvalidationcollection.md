##GridValidationCollection
Encapsulates a collection of  objects.
**Inheritance:**
java.lang.Object
```
public class GridValidationCollection
```
Encapsulates a collection of [GridValidation](../../com.aspose.gridweb/gridvalidation) objects.
## Methods
| Method | Description |
| --- | --- |
| [add()](#add--) | Add a [GridValidation](../../com.aspose.gridweb/gridvalidation) to the collection. |
| [add(GridCellArea ca)](#add-com.aspose.gridweb.GridCellArea-) | Adds a data validation to the collection. |
| [add(GridValidation validation)](#add-com.aspose.gridweb.GridValidation-) | Add a [GridValidation](../../com.aspose.gridweb/gridvalidation) to the collection. |
| [add(int row, int column)](#add-int-int-) | Add a [GridValidation](../../com.aspose.gridweb/gridvalidation) to the collection.the validation is applied to the specificed cell. |
| [add(String cellname)](#add-java.lang.String-) | Add a [GridValidation](../../com.aspose.gridweb/gridvalidation) to the collection.the validation is applied to the specificed cell. |
| [clear()](#clear--) | Clears all validations. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [get(int index)](#get-int-) | Gets the [GridValidation](../../com.aspose.gridweb/gridvalidation) element at the specified index. |
| [getClass()](#getClass--) |  |
| [getCount()](#getCount--) | Gets the size of enumerator |
| [getValidationInCell(int row, int column)](#getValidationInCell-int-int-) | Gets the validation applied to given cell. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeAt(int index)](#removeAt-int-) | Remove the validation at the specified index. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### add() {#add--}
```
public GridValidation add()
```
Add a [GridValidation](../../com.aspose.gridweb/gridvalidation) to the collection.
**Remarks**
NOTE: This member is now obsolete. Instead, please use GridValidationCollection.Add(row,col) method. This property will be removed 12 months later since JANUARY 2015. Aspose apologizes for any inconvenience you may have experienced.
**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(GridCellArea ca) {#add-com.aspose.gridweb.GridCellArea-}
```
public GridValidation add(GridCellArea ca)
```
Adds a data validation to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [GridCellArea](../../com.aspose.gridweb/gridcellarea) | The area contains this validation. |
**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the validation.
### add(GridValidation validation) {#add-com.aspose.gridweb.GridValidation-}
```
public int add(GridValidation validation)
```
Add a [GridValidation](../../com.aspose.gridweb/gridvalidation) to the collection.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| validation | [GridValidation](../../com.aspose.gridweb/gridvalidation) | A validation object. |
**Returns:**
int - [GridValidation](../../com.aspose.gridweb/gridvalidation) object index.
### add(int row, int column) {#add-int-int-}
```
public GridValidation add(int row, int column)
```
Add a [GridValidation](../../com.aspose.gridweb/gridvalidation) to the collection.the validation is applied to the specificed cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |
**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### add(String cellname) {#add-java.lang.String-}
```
public GridValidation add(String cellname)
```
Add a [GridValidation](../../com.aspose.gridweb/gridvalidation) to the collection.the validation is applied to the specificed cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| cellname | java.lang.String | the name of the cell. |
**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - [GridValidation](../../com.aspose.gridweb/gridvalidation) the added GridValidation instance.
### clear() {#clear--}
```
public void clear()
```
Clears all validations.
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
### get(int index) {#get-int-}
```
public GridValidation get(int index)
```
Gets the [GridValidation](../../com.aspose.gridweb/gridvalidation) element at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - The element at the specified index.
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getCount() {#getCount--}
```
public int getCount()
```
Gets the size of enumerator
**Returns:**
int
### getValidationInCell(int row, int column) {#getValidationInCell-int-int-}
```
public GridValidation getValidationInCell(int row, int column)
```
Gets the validation applied to given cell.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| row | int | The row index. |
| column | int | The column index. |
**Returns:**
[GridValidation](../../com.aspose.gridweb/gridvalidation) - Returns a [GridValidation](../../com.aspose.gridweb/gridvalidation) object or null if there is no validation for given cell
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
### removeAt(int index) {#removeAt-int-}
```
public void removeAt(int index)
```
Remove the validation at the specified index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | The zero based index of the element. |
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
