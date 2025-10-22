##DeleteBlankOptions
Represents the setting of deleting blank cells/rows/columns.
**Inheritance:**
java.lang.Object, [com.aspose.cells.DeleteOptions](../../com.aspose.cells/deleteoptions)
```
public class DeleteBlankOptions extends DeleteOptions
```
Represents the setting of deleting blank cells/rows/columns.
## Constructors
| Constructor | Description |
| --- | --- |
| [DeleteBlankOptions()](#DeleteBlankOptions--) |  |
## Methods
| Method | Description |
| --- | --- |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getClass()](#getClass--) |  |
| [getDrawingsAsBlank()](#getDrawingsAsBlank--) | Whether drawing related objects such as picture, shape, chart... will be taken as blank. |
| [getEmptyFormulaValueAsBlank()](#getEmptyFormulaValueAsBlank--) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. |
| [getEmptyStringAsBlank()](#getEmptyStringAsBlank--) | Whether one cell will be taken as blank when its value is empty string. |
| [getEndIndex()](#getEndIndex--) | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. |
| [getFormulaChangeMonitor()](#getFormulaChangeMonitor--) | Gets the monitor for tracking changes caused by the deletion. |
| [getMergedCellsShrinkType()](#getMergedCellsShrinkType--) | Indicates how to process merged cells when deleting blank rows/columns. |
| [getStartIndex()](#getStartIndex--) | Specifies the start row/column index of the range to check and delete blank rows/columns. |
| [getUpdateReference()](#getUpdateReference--) | Indicates if update references in other worksheets. |
| [hashCode()](#hashCode--) |  |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setDrawingsAsBlank(boolean value)](#setDrawingsAsBlank-boolean-) | Whether drawing related objects such as picture, shape, chart... will be taken as blank. |
| [setEmptyFormulaValueAsBlank(boolean value)](#setEmptyFormulaValueAsBlank-boolean-) | Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. |
| [setEmptyStringAsBlank(boolean value)](#setEmptyStringAsBlank-boolean-) | Whether one cell will be taken as blank when its value is empty string. |
| [setEndIndex(int value)](#setEndIndex-int-) | Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. |
| [setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)](#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-) | Sets the monitor for tracking changes caused by the deletion. |
| [setMergedCellsShrinkType(int value)](#setMergedCellsShrinkType-int-) | Indicates how to process merged cells when deleting blank rows/columns. |
| [setStartIndex(int value)](#setStartIndex-int-) | Specifies the start row/column index of the range to check and delete blank rows/columns. |
| [setUpdateReference(boolean value)](#setUpdateReference-boolean-) | Indicates if update references in other worksheets. |
| [toString()](#toString--) |  |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### DeleteBlankOptions() {#DeleteBlankOptions--}
```
public DeleteBlankOptions()
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
### getDrawingsAsBlank() {#getDrawingsAsBlank--}
```
public boolean getDrawingsAsBlank()
```
Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.
**Remarks**
When setting this property as false, all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.
**Returns:**
boolean
### getEmptyFormulaValueAsBlank() {#getEmptyFormulaValueAsBlank--}
```
public boolean getEmptyFormulaValueAsBlank()
```
Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false.
**Remarks**
Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) will be taken as blank and may be deleted because before calculation their calculated results are all null.
**Returns:**
boolean
### getEmptyStringAsBlank() {#getEmptyStringAsBlank--}
```
public boolean getEmptyStringAsBlank()
```
Whether one cell will be taken as blank when its value is empty string. Default value is true.
**Returns:**
boolean
### getEndIndex() {#getEndIndex--}
```
public int getEndIndex()
```
Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.
**Returns:**
int
### getFormulaChangeMonitor() {#getFormulaChangeMonitor--}
```
public AbstractFormulaChangeMonitor getFormulaChangeMonitor()
```
Gets the monitor for tracking changes caused by the deletion.
**Returns:**
[AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor)
### getMergedCellsShrinkType() {#getMergedCellsShrinkType--}
```
public int getMergedCellsShrinkType()
```
Indicates how to process merged cells when deleting blank rows/columns.
See [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).
**Remarks**
For [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.
For [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE), all cells in it will be taken as non-blank.
For [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT), all cells outside the content display area will be taken as blank.
**Returns:**
int
### getStartIndex() {#getStartIndex--}
```
public int getStartIndex()
```
Specifies the start row/column index of the range to check and delete blank rows/columns.
**Returns:**
int
### getUpdateReference() {#getUpdateReference--}
```
public boolean getUpdateReference()
```
Indicates if update references in other worksheets.
**Returns:**
boolean
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
### setDrawingsAsBlank(boolean value) {#setDrawingsAsBlank-boolean-}
```
public void setDrawingsAsBlank(boolean value)
```
Whether drawing related objects such as picture, shape, chart... will be taken as blank. Default value is true.
**Remarks**
When setting this property as false, all rows/columns covered by drawing objects will not be taken as blank and will not be deleted.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEmptyFormulaValueAsBlank(boolean value) {#setEmptyFormulaValueAsBlank-boolean-}
```
public void setEmptyFormulaValueAsBlank(boolean value)
```
Whether one cell will be taken as blank when it is formula and the calculated result is null or empty string. Default value is false.
**Remarks**
Generally user should make sure the formulas have been calculated before deleting operation with this property as true. Otherwise all newly cretaed formulas by normal apis such as [Cell.getFormula()](../../com.aspose.cells/cell\#getFormula--) will be taken as blank and may be deleted because before calculation their calculated results are all null.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEmptyStringAsBlank(boolean value) {#setEmptyStringAsBlank-boolean-}
```
public void setEmptyStringAsBlank(boolean value)
```
Whether one cell will be taken as blank when its value is empty string. Default value is true.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setEndIndex(int value) {#setEndIndex-int-}
```
public void setEndIndex(int value)
```
Specifies the end row/column index(inclusive) of the range to check and delete blank rows/columns. Default value is -1 and -1 means the maximum range of all objects(cells, drawings, ...) that need to be checked.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setFormulaChangeMonitor(AbstractFormulaChangeMonitor value) {#setFormulaChangeMonitor-com.aspose.cells.AbstractFormulaChangeMonitor-}
```
public void setFormulaChangeMonitor(AbstractFormulaChangeMonitor value)
```
Sets the monitor for tracking changes caused by the deletion.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | [AbstractFormulaChangeMonitor](../../com.aspose.cells/abstractformulachangemonitor) |  |
### setMergedCellsShrinkType(int value) {#setMergedCellsShrinkType-int-}
```
public void setMergedCellsShrinkType(int value)
```
Indicates how to process merged cells when deleting blank rows/columns.
See [MergedCellsShrinkType](../../com.aspose.cells/mergedcellsshrinktype).
**Remarks**
For [MergedCellsShrinkType.KEEP\_HEADER\_ONLY](../../com.aspose.cells/mergedcellsshrinktype\#KEEP-HEADER-ONLY), all cells in it will be taken as blank except the non-blank top-left cell. It is the default value of this property.
For [MergedCellsShrinkType.NONE](../../com.aspose.cells/mergedcellsshrinktype\#NONE), all cells in it will be taken as non-blank.
For [MergedCellsShrinkType.SHRINK\_TO\_FIT](../../com.aspose.cells/mergedcellsshrinktype\#SHRINK-TO-FIT), all cells outside the content display area will be taken as blank.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setStartIndex(int value) {#setStartIndex-int-}
```
public void setStartIndex(int value)
```
Specifies the start row/column index of the range to check and delete blank rows/columns.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | int |  |
### setUpdateReference(boolean value) {#setUpdateReference-boolean-}
```
public void setUpdateReference(boolean value)
```
Indicates if update references in other worksheets.
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
