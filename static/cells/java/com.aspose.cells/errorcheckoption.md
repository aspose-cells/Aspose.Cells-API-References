##ErrorCheckOption
Error check setting applied on certain ranges.
**Inheritance:**
java.lang.Object
```
public class ErrorCheckOption
```
Error check setting applied on certain ranges.
**Example**
```
Workbook workbook = new Workbook();
ErrorCheckOptionCollection opts = workbook.getWorksheets().get(0).getErrorCheckOptions();
int optionIdx = opts.add();
ErrorCheckOption opt = opts.get(optionIdx);
opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_FORMULA, false);
opt.setErrorCheck(com.aspose.cells.ErrorCheckType.INCONSIST_RANGE, false);
opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_DATE, false);
opt.setErrorCheck(com.aspose.cells.ErrorCheckType.TEXT_NUMBER, false);
opt.setErrorCheck(com.aspose.cells.ErrorCheckType.VALIDATION, false);
opt.addRange(CellArea.createCellArea("A1", "B10"));
workbook.save("Book1.xlsx");
```
## Methods
| Method | Description |
| --- | --- |
| [addRange(CellArea ca)](#addRange-com.aspose.cells.CellArea-) | Adds one influenced range by this setting. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getCountOfRange()](#getCountOfRange--) | Gets the count of ranges that influenced by this setting. |
| [getRange(int index)](#getRange-int-) | Gets the influenced range of this setting by given index. |
| [hashCode()](#hashCode--) |  |
| [isErrorCheck(int errorCheckType)](#isErrorCheck-int-) | Checks whether given error type will be checked. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [removeRange(int index)](#removeRange-int-) | Removes one range by given index. |
| [setErrorCheck(int errorCheckType, boolean isCheck)](#setErrorCheck-int-boolean-) | Sets whether given error type will be checked. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### addRange(CellArea ca) {#addRange-com.aspose.cells.CellArea-}
```
public int addRange(CellArea ca)
```
Adds one influenced range by this setting.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| ca | [CellArea](../../com.aspose.cells/cellarea) | the range to be added. |
**Returns:**
int - the index of the added range in the range list of this setting.
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
### getCountOfRange() {#getCountOfRange--}
```
public int getCountOfRange()
```
Gets the count of ranges that influenced by this setting.
**Returns:**
int - the count of ranges that influenced by this setting.
### getRange(int index) {#getRange-int-}
```
public CellArea getRange(int index)
```
Gets the influenced range of this setting by given index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of range |
**Returns:**
[CellArea](../../com.aspose.cells/cellarea) - return influenced range at given index.
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isErrorCheck(int errorCheckType) {#isErrorCheck-int-}
```
public boolean isErrorCheck(int errorCheckType)
```
Checks whether given error type will be checked.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). error type can be checked |
**Returns:**
boolean - return true if given error type will be checked(green triangle will be shown for cell if the check failed).
### notify() {#notify--}
```
public final native void notify()
```
### notifyAll() {#notifyAll--}
```
public final native void notifyAll()
```
### removeRange(int index) {#removeRange-int-}
```
public void removeRange(int index)
```
Removes one range by given index.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| index | int | the index of the range to be removed. |
### setErrorCheck(int errorCheckType, boolean isCheck) {#setErrorCheck-int-boolean-}
```
public void setErrorCheck(int errorCheckType, boolean isCheck)
```
Sets whether given error type will be checked.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| errorCheckType | int | [ErrorCheckType](../../com.aspose.cells/errorchecktype). error type can be checked. |
| isCheck | boolean | true if given error type needs to be checked(green triangle will be shown for cell if the check failed). |
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
