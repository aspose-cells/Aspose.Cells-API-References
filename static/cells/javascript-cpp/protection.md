##Protection
Represents the various types of protection options available for a worksheet.
## Protection class
Represents the various types of protection options available for a worksheet.
```javascript
class Protection;
```
### Example
```javascript
const { Workbook } = AsposeCells;
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
| [copy(Protection)](#copy-protection-)| Copy protection info. |
| [verifyPassword(string)](#verifyPassword-string-)| Verifies password. |
| [getPasswordHash()](#getPasswordHash--)| Gets the hash of current password. |
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
