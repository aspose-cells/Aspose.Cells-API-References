##Protection
Represents the various types of protection options available for a worksheet.
## Protection class
Represents the various types of protection options available for a worksheet.
```javascript
class Protection;
```
### Example
```javascript
const { Workbook } = require("aspose.cells.node");
var workbook = new Workbook();
var sheetIndex = workbook.worksheets.add();
var worksheet = workbook.worksheets.get(sheetIndex);
//Allowing users to select locked cells of the worksheet
worksheet.protection.allowSelectingLockedCell = true;
//Allowing users to select unlocked cells of the worksheet
worksheet.protection.allowSelectingUnlockedCell = true;
```
## Properties
| Property | Type | Description |
| --- | --- | --- |
| [allowDeletingColumn](#allowDeletingColumn--)| boolean | Represents if the deletion of columns is allowed on a protected worksheet. |
| [allowDeletingRow](#allowDeletingRow--)| boolean | Represents if the deletion of rows is allowed on a protected worksheet. |
| [allowFiltering](#allowFiltering--)| boolean | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [allowFormattingCell](#allowFormattingCell--)| boolean | Represents if the formatting of cells is allowed on a protected worksheet. |
| [allowFormattingColumn](#allowFormattingColumn--)| boolean | Represents if the formatting of columns is allowed on a protected worksheet |
| [allowFormattingRow](#allowFormattingRow--)| boolean | Represents if the formatting of rows is allowed on a protected worksheet |
| [allowInsertingColumn](#allowInsertingColumn--)| boolean | Represents if the insertion of columns is allowed on a protected worksheet |
| [allowInsertingHyperlink](#allowInsertingHyperlink--)| boolean | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [allowInsertingRow](#allowInsertingRow--)| boolean | Represents if the insertion of rows is allowed on a protected worksheet |
| [allowSorting](#allowSorting--)| boolean | Represents if the sorting option is allowed on a protected worksheet. |
| [allowUsingPivotTable](#allowUsingPivotTable--)| boolean | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [allowEditingContent](#allowEditingContent--)| boolean | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [allowEditingObject](#allowEditingObject--)| boolean | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [allowEditingScenario](#allowEditingScenario--)| boolean | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [allowSelectingLockedCell](#allowSelectingLockedCell--)| boolean | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [allowSelectingUnlockedCell](#allowSelectingUnlockedCell--)| boolean | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [password](#password--)| string | Represents the password to protect the worksheet. |
| [isProtectedWithPassword](#isProtectedWithPassword--)| boolean | Readonly. Indicates whether the worksheets is protected with password. |
## Methods
| Method | Description |
| --- | --- |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--)| <b>@deprecated.</b> Please use the 'allowDeletingColumn' property instead. Represents if the deletion of columns is allowed on a protected worksheet. |
| [setAllowDeletingColumn(boolean)](#setAllowDeletingColumn-boolean-)| <b>@deprecated.</b> Please use the 'allowDeletingColumn' property instead. Represents if the deletion of columns is allowed on a protected worksheet. |
| [getAllowDeletingRow()](#getAllowDeletingRow--)| <b>@deprecated.</b> Please use the 'allowDeletingRow' property instead. Represents if the deletion of rows is allowed on a protected worksheet. |
| [setAllowDeletingRow(boolean)](#setAllowDeletingRow-boolean-)| <b>@deprecated.</b> Please use the 'allowDeletingRow' property instead. Represents if the deletion of rows is allowed on a protected worksheet. |
| [getAllowFiltering()](#getAllowFiltering--)| <b>@deprecated.</b> Please use the 'allowFiltering' property instead. Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [setAllowFiltering(boolean)](#setAllowFiltering-boolean-)| <b>@deprecated.</b> Please use the 'allowFiltering' property instead. Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [getAllowFormattingCell()](#getAllowFormattingCell--)| <b>@deprecated.</b> Please use the 'allowFormattingCell' property instead. Represents if the formatting of cells is allowed on a protected worksheet. |
| [setAllowFormattingCell(boolean)](#setAllowFormattingCell-boolean-)| <b>@deprecated.</b> Please use the 'allowFormattingCell' property instead. Represents if the formatting of cells is allowed on a protected worksheet. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--)| <b>@deprecated.</b> Please use the 'allowFormattingColumn' property instead. Represents if the formatting of columns is allowed on a protected worksheet |
| [setAllowFormattingColumn(boolean)](#setAllowFormattingColumn-boolean-)| <b>@deprecated.</b> Please use the 'allowFormattingColumn' property instead. Represents if the formatting of columns is allowed on a protected worksheet |
| [getAllowFormattingRow()](#getAllowFormattingRow--)| <b>@deprecated.</b> Please use the 'allowFormattingRow' property instead. Represents if the formatting of rows is allowed on a protected worksheet |
| [setAllowFormattingRow(boolean)](#setAllowFormattingRow-boolean-)| <b>@deprecated.</b> Please use the 'allowFormattingRow' property instead. Represents if the formatting of rows is allowed on a protected worksheet |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--)| <b>@deprecated.</b> Please use the 'allowInsertingColumn' property instead. Represents if the insertion of columns is allowed on a protected worksheet |
| [setAllowInsertingColumn(boolean)](#setAllowInsertingColumn-boolean-)| <b>@deprecated.</b> Please use the 'allowInsertingColumn' property instead. Represents if the insertion of columns is allowed on a protected worksheet |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--)| <b>@deprecated.</b> Please use the 'allowInsertingHyperlink' property instead. Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [setAllowInsertingHyperlink(boolean)](#setAllowInsertingHyperlink-boolean-)| <b>@deprecated.</b> Please use the 'allowInsertingHyperlink' property instead. Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [getAllowInsertingRow()](#getAllowInsertingRow--)| <b>@deprecated.</b> Please use the 'allowInsertingRow' property instead. Represents if the insertion of rows is allowed on a protected worksheet |
| [setAllowInsertingRow(boolean)](#setAllowInsertingRow-boolean-)| <b>@deprecated.</b> Please use the 'allowInsertingRow' property instead. Represents if the insertion of rows is allowed on a protected worksheet |
| [getAllowSorting()](#getAllowSorting--)| <b>@deprecated.</b> Please use the 'allowSorting' property instead. Represents if the sorting option is allowed on a protected worksheet. |
| [setAllowSorting(boolean)](#setAllowSorting-boolean-)| <b>@deprecated.</b> Please use the 'allowSorting' property instead. Represents if the sorting option is allowed on a protected worksheet. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--)| <b>@deprecated.</b> Please use the 'allowUsingPivotTable' property instead. Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [setAllowUsingPivotTable(boolean)](#setAllowUsingPivotTable-boolean-)| <b>@deprecated.</b> Please use the 'allowUsingPivotTable' property instead. Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [getAllowEditingContent()](#getAllowEditingContent--)| <b>@deprecated.</b> Please use the 'allowEditingContent' property instead. Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [setAllowEditingContent(boolean)](#setAllowEditingContent-boolean-)| <b>@deprecated.</b> Please use the 'allowEditingContent' property instead. Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [getAllowEditingObject()](#getAllowEditingObject--)| <b>@deprecated.</b> Please use the 'allowEditingObject' property instead. Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [setAllowEditingObject(boolean)](#setAllowEditingObject-boolean-)| <b>@deprecated.</b> Please use the 'allowEditingObject' property instead. Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [getAllowEditingScenario()](#getAllowEditingScenario--)| <b>@deprecated.</b> Please use the 'allowEditingScenario' property instead. Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [setAllowEditingScenario(boolean)](#setAllowEditingScenario-boolean-)| <b>@deprecated.</b> Please use the 'allowEditingScenario' property instead. Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--)| <b>@deprecated.</b> Please use the 'allowSelectingLockedCell' property instead. Represents if the user is allowed to select locked cells on a protected worksheet. |
| [setAllowSelectingLockedCell(boolean)](#setAllowSelectingLockedCell-boolean-)| <b>@deprecated.</b> Please use the 'allowSelectingLockedCell' property instead. Represents if the user is allowed to select locked cells on a protected worksheet. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--)| <b>@deprecated.</b> Please use the 'allowSelectingUnlockedCell' property instead. Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [setAllowSelectingUnlockedCell(boolean)](#setAllowSelectingUnlockedCell-boolean-)| <b>@deprecated.</b> Please use the 'allowSelectingUnlockedCell' property instead. Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [getPassword()](#getPassword--)| <b>@deprecated.</b> Please use the 'password' property instead. Represents the password to protect the worksheet. |
| [setPassword(string)](#setPassword-string-)| <b>@deprecated.</b> Please use the 'password' property instead. Represents the password to protect the worksheet. |
| [isProtectedWithPassword()](#isProtectedWithPassword--)| <b>@deprecated.</b> Please use the 'isProtectedWithPassword' property instead. Indicates whether the worksheets is protected with password. |
| [copy(Protection)](#copy-protection-)| Copy protection info. |
| [verifyPassword(string)](#verifyPassword-string-)| Verifies password. |
| [getPasswordHash()](#getPasswordHash--)| Gets the hash of current password. |
| [isNull()](#isNull--)| Checks whether the implementation object is null. |
### allowDeletingColumn {#allowDeletingColumn--}
Represents if the deletion of columns is allowed on a protected worksheet.
```javascript
allowDeletingColumn : boolean;
```
**Remarks**
The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
### allowDeletingRow {#allowDeletingRow--}
Represents if the deletion of rows is allowed on a protected worksheet.
```javascript
allowDeletingRow : boolean;
```
**Remarks**
The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
### allowFiltering {#allowFiltering--}
Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.
```javascript
allowFiltering : boolean;
```
### allowFormattingCell {#allowFormattingCell--}
Represents if the formatting of cells is allowed on a protected worksheet.
```javascript
allowFormattingCell : boolean;
```
### allowFormattingColumn {#allowFormattingColumn--}
Represents if the formatting of columns is allowed on a protected worksheet
```javascript
allowFormattingColumn : boolean;
```
### allowFormattingRow {#allowFormattingRow--}
Represents if the formatting of rows is allowed on a protected worksheet
```javascript
allowFormattingRow : boolean;
```
### allowInsertingColumn {#allowInsertingColumn--}
Represents if the insertion of columns is allowed on a protected worksheet
```javascript
allowInsertingColumn : boolean;
```
### allowInsertingHyperlink {#allowInsertingHyperlink--}
Represents if the insertion of hyperlinks is allowed on a protected worksheet
```javascript
allowInsertingHyperlink : boolean;
```
### allowInsertingRow {#allowInsertingRow--}
Represents if the insertion of rows is allowed on a protected worksheet
```javascript
allowInsertingRow : boolean;
```
### allowSorting {#allowSorting--}
Represents if the sorting option is allowed on a protected worksheet.
```javascript
allowSorting : boolean;
```
### allowUsingPivotTable {#allowUsingPivotTable--}
Represents if the user is allowed to manipulate pivot tables on a protected worksheet.
```javascript
allowUsingPivotTable : boolean;
```
### allowEditingContent {#allowEditingContent--}
Represents if the user is allowed to edit contents of locked cells on a protected worksheet.
```javascript
allowEditingContent : boolean;
```
### allowEditingObject {#allowEditingObject--}
Represents if the user is allowed to manipulate drawing objects on a protected worksheet.
```javascript
allowEditingObject : boolean;
```
### allowEditingScenario {#allowEditingScenario--}
Represents if the user is allowed to edit scenarios on a protected worksheet.
```javascript
allowEditingScenario : boolean;
```
### allowSelectingLockedCell {#allowSelectingLockedCell--}
Represents if the user is allowed to select locked cells on a protected worksheet.
```javascript
allowSelectingLockedCell : boolean;
```
### allowSelectingUnlockedCell {#allowSelectingUnlockedCell--}
Represents if the user is allowed to select unlocked cells on a protected worksheet.
```javascript
allowSelectingUnlockedCell : boolean;
```
### password {#password--}
Represents the password to protect the worksheet.
```javascript
password : string;
```
**Remarks**
If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.
### isProtectedWithPassword {#isProtectedWithPassword--}
Readonly. Indicates whether the worksheets is protected with password.
```javascript
isProtectedWithPassword : boolean;
```
### getAllowDeletingColumn() {#getAllowDeletingColumn--}
```javascript
getAllowDeletingColumn() : boolean;
```
**Remarks**
The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
### setAllowDeletingColumn(boolean) {#setAllowDeletingColumn-boolean-}
```javascript
setAllowDeletingColumn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
### getAllowDeletingRow() {#getAllowDeletingRow--}
```javascript
getAllowDeletingRow() : boolean;
```
**Remarks**
The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
### setAllowDeletingRow(boolean) {#setAllowDeletingRow-boolean-}
```javascript
setAllowDeletingRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
**Remarks**
The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.
### getAllowFiltering() {#getAllowFiltering--}
```javascript
getAllowFiltering() : boolean;
```
### setAllowFiltering(boolean) {#setAllowFiltering-boolean-}
```javascript
setAllowFiltering(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowFormattingCell() {#getAllowFormattingCell--}
```javascript
getAllowFormattingCell() : boolean;
```
### setAllowFormattingCell(boolean) {#setAllowFormattingCell-boolean-}
```javascript
setAllowFormattingCell(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowFormattingColumn() {#getAllowFormattingColumn--}
```javascript
getAllowFormattingColumn() : boolean;
```
### setAllowFormattingColumn(boolean) {#setAllowFormattingColumn-boolean-}
```javascript
setAllowFormattingColumn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowFormattingRow() {#getAllowFormattingRow--}
```javascript
getAllowFormattingRow() : boolean;
```
### setAllowFormattingRow(boolean) {#setAllowFormattingRow-boolean-}
```javascript
setAllowFormattingRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowInsertingColumn() {#getAllowInsertingColumn--}
```javascript
getAllowInsertingColumn() : boolean;
```
### setAllowInsertingColumn(boolean) {#setAllowInsertingColumn-boolean-}
```javascript
setAllowInsertingColumn(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}
```javascript
getAllowInsertingHyperlink() : boolean;
```
### setAllowInsertingHyperlink(boolean) {#setAllowInsertingHyperlink-boolean-}
```javascript
setAllowInsertingHyperlink(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowInsertingRow() {#getAllowInsertingRow--}
```javascript
getAllowInsertingRow() : boolean;
```
### setAllowInsertingRow(boolean) {#setAllowInsertingRow-boolean-}
```javascript
setAllowInsertingRow(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowSorting() {#getAllowSorting--}
```javascript
getAllowSorting() : boolean;
```
### setAllowSorting(boolean) {#setAllowSorting-boolean-}
```javascript
setAllowSorting(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}
```javascript
getAllowUsingPivotTable() : boolean;
```
### setAllowUsingPivotTable(boolean) {#setAllowUsingPivotTable-boolean-}
```javascript
setAllowUsingPivotTable(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowEditingContent() {#getAllowEditingContent--}
```javascript
getAllowEditingContent() : boolean;
```
### setAllowEditingContent(boolean) {#setAllowEditingContent-boolean-}
```javascript
setAllowEditingContent(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowEditingObject() {#getAllowEditingObject--}
```javascript
getAllowEditingObject() : boolean;
```
### setAllowEditingObject(boolean) {#setAllowEditingObject-boolean-}
```javascript
setAllowEditingObject(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowEditingScenario() {#getAllowEditingScenario--}
```javascript
getAllowEditingScenario() : boolean;
```
### setAllowEditingScenario(boolean) {#setAllowEditingScenario-boolean-}
```javascript
setAllowEditingScenario(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}
```javascript
getAllowSelectingLockedCell() : boolean;
```
### setAllowSelectingLockedCell(boolean) {#setAllowSelectingLockedCell-boolean-}
```javascript
setAllowSelectingLockedCell(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}
```javascript
getAllowSelectingUnlockedCell() : boolean;
```
### setAllowSelectingUnlockedCell(boolean) {#setAllowSelectingUnlockedCell-boolean-}
```javascript
setAllowSelectingUnlockedCell(value: boolean) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |
### getPassword() {#getPassword--}
```javascript
getPassword() : string;
```
**Remarks**
If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.
### setPassword(string) {#setPassword-string-}
```javascript
setPassword(value: string) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | string | The value to set. |
**Remarks**
If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.
### isProtectedWithPassword() {#isProtectedWithPassword--}
```javascript
isProtectedWithPassword() : boolean;
```
### copy(Protection) {#copy-protection-}
Copy protection info.
```javascript
copy(source: Protection) : void;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Protection](../protection/) |  |
### verifyPassword(string) {#verifyPassword-string-}
Verifies password.
```javascript
verifyPassword(password: string) : boolean;
```
**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | The password. |
### getPasswordHash() {#getPasswordHash--}
Gets the hash of current password.
```javascript
getPasswordHash() : number;
```
### isNull() {#isNull--}
Checks whether the implementation object is null.
```javascript
isNull() : boolean;
```
