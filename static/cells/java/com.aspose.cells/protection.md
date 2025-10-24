##Protection
Represents the various types of protection options available for a worksheet.
**Inheritance:**
java.lang.Object
```
public class Protection
```
Represents the various types of protection options available for a worksheet.
**Example**
```
//Instantiating a Workbook object
Workbook workbook = new Workbook();
Worksheet worksheet = workbook.getWorksheets().get(0);
//Allowing users to select locked cells of the worksheet
worksheet.getProtection().setAllowSelectingLockedCell(true);
//Allowing users to select unlocked cells of the worksheet
worksheet.getProtection().setAllowSelectingUnlockedCell(true);
```
## Methods
| Method | Description |
| --- | --- |
| [copy(Protection source)](#copy-com.aspose.cells.Protection-) | Copy protection info. |
| [equals(Object arg0)](#equals-java.lang.Object-) |  |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [getAllowDeletingRow()](#getAllowDeletingRow--) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [getAllowEditingContent()](#getAllowEditingContent--) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [getAllowEditingObject()](#getAllowEditingObject--) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [getAllowEditingScenario()](#getAllowEditingScenario--) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [getAllowFiltering()](#getAllowFiltering--) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [getAllowFormattingCell()](#getAllowFormattingCell--) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--) | Represents if the formatting of columns is allowed on a protected worksheet |
| [getAllowFormattingRow()](#getAllowFormattingRow--) | Represents if the formatting of rows is allowed on a protected worksheet |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--) | Represents if the insertion of columns is allowed on a protected worksheet |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--) | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [getAllowInsertingRow()](#getAllowInsertingRow--) | Represents if the insertion of rows is allowed on a protected worksheet |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [getAllowSorting()](#getAllowSorting--) | Represents if the sorting option is allowed on a protected worksheet. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [getClass()](#getClass--) |  |
| [getPassword()](#getPassword--) | Represents the password to protect the worksheet. |
| [getPasswordHash()](#getPasswordHash--) | Gets the hash of current password. |
| [hashCode()](#hashCode--) |  |
| [isProtectedWithPassword()](#isProtectedWithPassword--) | Indicates whether the worksheets is protected with password. |
| [notify()](#notify--) |  |
| [notifyAll()](#notifyAll--) |  |
| [setAllowDeletingColumn(boolean value)](#setAllowDeletingColumn-boolean-) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [setAllowDeletingRow(boolean value)](#setAllowDeletingRow-boolean-) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [setAllowEditingContent(boolean value)](#setAllowEditingContent-boolean-) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [setAllowEditingObject(boolean value)](#setAllowEditingObject-boolean-) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [setAllowEditingScenario(boolean value)](#setAllowEditingScenario-boolean-) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [setAllowFiltering(boolean value)](#setAllowFiltering-boolean-) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [setAllowFormattingCell(boolean value)](#setAllowFormattingCell-boolean-) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [setAllowFormattingColumn(boolean value)](#setAllowFormattingColumn-boolean-) | Represents if the formatting of columns is allowed on a protected worksheet |
| [setAllowFormattingRow(boolean value)](#setAllowFormattingRow-boolean-) | Represents if the formatting of rows is allowed on a protected worksheet |
| [setAllowInsertingColumn(boolean value)](#setAllowInsertingColumn-boolean-) | Represents if the insertion of columns is allowed on a protected worksheet |
| [setAllowInsertingHyperlink(boolean value)](#setAllowInsertingHyperlink-boolean-) | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [setAllowInsertingRow(boolean value)](#setAllowInsertingRow-boolean-) | Represents if the insertion of rows is allowed on a protected worksheet |
| [setAllowSelectingLockedCell(boolean value)](#setAllowSelectingLockedCell-boolean-) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [setAllowSelectingUnlockedCell(boolean value)](#setAllowSelectingUnlockedCell-boolean-) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [setAllowSorting(boolean value)](#setAllowSorting-boolean-) | Represents if the sorting option is allowed on a protected worksheet. |
| [setAllowUsingPivotTable(boolean value)](#setAllowUsingPivotTable-boolean-) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [setPassword(String value)](#setPassword-java.lang.String-) | Represents the password to protect the worksheet. |
| [toString()](#toString--) |  |
| [verifyPassword(String password)](#verifyPassword-java.lang.String-) | Verifies password. |
| [wait()](#wait--) |  |
| [wait(long arg0)](#wait-long-) |  |
| [wait(long arg0, int arg1)](#wait-long-int-) |  |
### copy(Protection source) {#copy-com.aspose.cells.Protection-}
```
public void copy(Protection source)
```
Copy protection info.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Protection](../../com.aspose.cells/protection) |  |
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
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```
public boolean getAllowDeletingColumn()
```
Represents if the deletion of columns is allowed on a protected worksheet.
**Remarks**
The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
**Returns:**
boolean
### getAllowDeletingRow() {#getAllowDeletingRow--}
```
public boolean getAllowDeletingRow()
```
Represents if the deletion of rows is allowed on a protected worksheet.
**Remarks**
The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
**Returns:**
boolean
### getAllowEditingContent() {#getAllowEditingContent--}
```
public boolean getAllowEditingContent()
```
Represents if the user is allowed to edit contents of locked cells on a protected worksheet.
**Returns:**
boolean
### getAllowEditingObject() {#getAllowEditingObject--}
```
public boolean getAllowEditingObject()
```
Represents if the user is allowed to manipulate drawing objects on a protected worksheet.
**Returns:**
boolean
### getAllowEditingScenario() {#getAllowEditingScenario--}
```
public boolean getAllowEditingScenario()
```
Represents if the user is allowed to edit scenarios on a protected worksheet.
**Returns:**
boolean
### getAllowFiltering() {#getAllowFiltering--}
```
public boolean getAllowFiltering()
```
Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.
**Returns:**
boolean
### getAllowFormattingCell() {#getAllowFormattingCell--}
```
public boolean getAllowFormattingCell()
```
Represents if the formatting of cells is allowed on a protected worksheet.
**Returns:**
boolean
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```
public boolean getAllowFormattingColumn()
```
Represents if the formatting of columns is allowed on a protected worksheet
**Returns:**
boolean
### getAllowFormattingRow() {#getAllowFormattingRow--}
```
public boolean getAllowFormattingRow()
```
Represents if the formatting of rows is allowed on a protected worksheet
**Returns:**
boolean
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```
public boolean getAllowInsertingColumn()
```
Represents if the insertion of columns is allowed on a protected worksheet
**Returns:**
boolean
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```
public boolean getAllowInsertingHyperlink()
```
Represents if the insertion of hyperlinks is allowed on a protected worksheet
**Returns:**
boolean
### getAllowInsertingRow() {#getAllowInsertingRow--}
```
public boolean getAllowInsertingRow()
```
Represents if the insertion of rows is allowed on a protected worksheet
**Returns:**
boolean
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```
public boolean getAllowSelectingLockedCell()
```
Represents if the user is allowed to select locked cells on a protected worksheet.
**Returns:**
boolean
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```
public boolean getAllowSelectingUnlockedCell()
```
Represents if the user is allowed to select unlocked cells on a protected worksheet.
**Returns:**
boolean
### getAllowSorting() {#getAllowSorting--}
```
public boolean getAllowSorting()
```
Represents if the sorting option is allowed on a protected worksheet.
**Returns:**
boolean
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```
public boolean getAllowUsingPivotTable()
```
Represents if the user is allowed to manipulate pivot tables on a protected worksheet.
**Returns:**
boolean
### getClass() {#getClass--}
```
public final native Class<?> getClass()
```
**Returns:**
java.lang.Class<?>
### getPassword() {#getPassword--}
```
public String getPassword()
```
Represents the password to protect the worksheet.
**Remarks**
If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.
**Returns:**
java.lang.String
### getPasswordHash() {#getPasswordHash--}
```
public int getPasswordHash()
```
Gets the hash of current password.
**Returns:**
int
### hashCode() {#hashCode--}
```
public native int hashCode()
```
**Returns:**
int
### isProtectedWithPassword() {#isProtectedWithPassword--}
```
public boolean isProtectedWithPassword()
```
Indicates whether the worksheets is protected with password.
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
### setAllowDeletingColumn(boolean value) {#setAllowDeletingColumn-boolean-}
```
public void setAllowDeletingColumn(boolean value)
```
Represents if the deletion of columns is allowed on a protected worksheet.
**Remarks**
The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowDeletingRow(boolean value) {#setAllowDeletingRow-boolean-}
```
public void setAllowDeletingRow(boolean value)
```
Represents if the deletion of rows is allowed on a protected worksheet.
**Remarks**
The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowEditingContent(boolean value) {#setAllowEditingContent-boolean-}
```
public void setAllowEditingContent(boolean value)
```
Represents if the user is allowed to edit contents of locked cells on a protected worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowEditingObject(boolean value) {#setAllowEditingObject-boolean-}
```
public void setAllowEditingObject(boolean value)
```
Represents if the user is allowed to manipulate drawing objects on a protected worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowEditingScenario(boolean value) {#setAllowEditingScenario-boolean-}
```
public void setAllowEditingScenario(boolean value)
```
Represents if the user is allowed to edit scenarios on a protected worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowFiltering(boolean value) {#setAllowFiltering-boolean-}
```
public void setAllowFiltering(boolean value)
```
Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowFormattingCell(boolean value) {#setAllowFormattingCell-boolean-}
```
public void setAllowFormattingCell(boolean value)
```
Represents if the formatting of cells is allowed on a protected worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowFormattingColumn(boolean value) {#setAllowFormattingColumn-boolean-}
```
public void setAllowFormattingColumn(boolean value)
```
Represents if the formatting of columns is allowed on a protected worksheet
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowFormattingRow(boolean value) {#setAllowFormattingRow-boolean-}
```
public void setAllowFormattingRow(boolean value)
```
Represents if the formatting of rows is allowed on a protected worksheet
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowInsertingColumn(boolean value) {#setAllowInsertingColumn-boolean-}
```
public void setAllowInsertingColumn(boolean value)
```
Represents if the insertion of columns is allowed on a protected worksheet
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowInsertingHyperlink(boolean value) {#setAllowInsertingHyperlink-boolean-}
```
public void setAllowInsertingHyperlink(boolean value)
```
Represents if the insertion of hyperlinks is allowed on a protected worksheet
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowInsertingRow(boolean value) {#setAllowInsertingRow-boolean-}
```
public void setAllowInsertingRow(boolean value)
```
Represents if the insertion of rows is allowed on a protected worksheet
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowSelectingLockedCell(boolean value) {#setAllowSelectingLockedCell-boolean-}
```
public void setAllowSelectingLockedCell(boolean value)
```
Represents if the user is allowed to select locked cells on a protected worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowSelectingUnlockedCell(boolean value) {#setAllowSelectingUnlockedCell-boolean-}
```
public void setAllowSelectingUnlockedCell(boolean value)
```
Represents if the user is allowed to select unlocked cells on a protected worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowSorting(boolean value) {#setAllowSorting-boolean-}
```
public void setAllowSorting(boolean value)
```
Represents if the sorting option is allowed on a protected worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setAllowUsingPivotTable(boolean value) {#setAllowUsingPivotTable-boolean-}
```
public void setAllowUsingPivotTable(boolean value)
```
Represents if the user is allowed to manipulate pivot tables on a protected worksheet.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean |  |
### setPassword(String value) {#setPassword-java.lang.String-}
```
public void setPassword(String value)
```
Represents the password to protect the worksheet.
**Remarks**
If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | java.lang.String |  |
### toString() {#toString--}
```
public String toString()
```
**Returns:**
java.lang.String
### verifyPassword(String password) {#verifyPassword-java.lang.String-}
```
public boolean verifyPassword(String password)
```
Verifies password.
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | java.lang.String | The password. |
**Returns:**
boolean -
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
