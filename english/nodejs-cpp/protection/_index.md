---
title: Protection
second_title: Aspose.Cells for Node.js via C++ API Reference
description: Represents the various types of protection options available for a worksheet.
type: docs
url: /nodejs-cpp/protection/
---

## Protection class

Represents the various types of protection options available for a worksheet.

```javascript
class Protection;
```


## Methods

| Method | Description |
| --- | --- |
| [getAllowDeletingColumn()](#getAllowDeletingColumn--)| Represents if the deletion of columns is allowed on a protected worksheet. |
| [setAllowDeletingColumn(boolean)](#setAllowDeletingColumn-boolean-)| Represents if the deletion of columns is allowed on a protected worksheet. |
| [getAllowDeletingRow()](#getAllowDeletingRow--)| Represents if the deletion of rows is allowed on a protected worksheet. |
| [setAllowDeletingRow(boolean)](#setAllowDeletingRow-boolean-)| Represents if the deletion of rows is allowed on a protected worksheet. |
| [getAllowFiltering()](#getAllowFiltering--)| Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [setAllowFiltering(boolean)](#setAllowFiltering-boolean-)| Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [getAllowFormattingCell()](#getAllowFormattingCell--)| Represents if the formatting of cells is allowed on a protected worksheet. |
| [setAllowFormattingCell(boolean)](#setAllowFormattingCell-boolean-)| Represents if the formatting of cells is allowed on a protected worksheet. |
| [getAllowFormattingColumn()](#getAllowFormattingColumn--)| Represents if the formatting of columns is allowed on a protected worksheet |
| [setAllowFormattingColumn(boolean)](#setAllowFormattingColumn-boolean-)| Represents if the formatting of columns is allowed on a protected worksheet |
| [getAllowFormattingRow()](#getAllowFormattingRow--)| Represents if the formatting of rows is allowed on a protected worksheet |
| [setAllowFormattingRow(boolean)](#setAllowFormattingRow-boolean-)| Represents if the formatting of rows is allowed on a protected worksheet |
| [getAllowInsertingColumn()](#getAllowInsertingColumn--)| Represents if the insertion of columns is allowed on a protected worksheet |
| [setAllowInsertingColumn(boolean)](#setAllowInsertingColumn-boolean-)| Represents if the insertion of columns is allowed on a protected worksheet |
| [getAllowInsertingHyperlink()](#getAllowInsertingHyperlink--)| Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [setAllowInsertingHyperlink(boolean)](#setAllowInsertingHyperlink-boolean-)| Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [getAllowInsertingRow()](#getAllowInsertingRow--)| Represents if the insertion of rows is allowed on a protected worksheet |
| [setAllowInsertingRow(boolean)](#setAllowInsertingRow-boolean-)| Represents if the insertion of rows is allowed on a protected worksheet |
| [getAllowSorting()](#getAllowSorting--)| Represents if the sorting option is allowed on a protected worksheet. |
| [setAllowSorting(boolean)](#setAllowSorting-boolean-)| Represents if the sorting option is allowed on a protected worksheet. |
| [getAllowUsingPivotTable()](#getAllowUsingPivotTable--)| Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [setAllowUsingPivotTable(boolean)](#setAllowUsingPivotTable-boolean-)| Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [getAllowEditingContent()](#getAllowEditingContent--)| Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [setAllowEditingContent(boolean)](#setAllowEditingContent-boolean-)| Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [getAllowEditingObject()](#getAllowEditingObject--)| Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [setAllowEditingObject(boolean)](#setAllowEditingObject-boolean-)| Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [getAllowEditingScenario()](#getAllowEditingScenario--)| Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [setAllowEditingScenario(boolean)](#setAllowEditingScenario-boolean-)| Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [getPassword()](#getPassword--)| Represents the password to protect the worksheet. |
| [setPassword(string)](#setPassword-string-)| Represents the password to protect the worksheet. |
| [isProtectedWithPassword()](#isProtectedWithPassword--)| Indicates whether the worksheets is protected with password. |
| [getAllowSelectingLockedCell()](#getAllowSelectingLockedCell--)| Represents if the user is allowed to select locked cells on a protected worksheet. |
| [setAllowSelectingLockedCell(boolean)](#setAllowSelectingLockedCell-boolean-)| Represents if the user is allowed to select locked cells on a protected worksheet. |
| [getAllowSelectingUnlockedCell()](#getAllowSelectingUnlockedCell--)| Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [setAllowSelectingUnlockedCell(boolean)](#setAllowSelectingUnlockedCell-boolean-)| Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [copy(Protection)](#copy-protection-)| Copy protection info. |
| [getPasswordHash()](#getPasswordHash--)| Gets the hash of current password. |
| [verifyPassword(string)](#verifyPassword-string-)| Verifies password. |


### getAllowDeletingColumn() {#getAllowDeletingColumn--}

Represents if the deletion of columns is allowed on a protected worksheet.

```javascript
getAllowDeletingColumn() : boolean;
```


**Remarks**

The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

### setAllowDeletingColumn(boolean) {#setAllowDeletingColumn-boolean-}

Represents if the deletion of columns is allowed on a protected worksheet.

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

Represents if the deletion of rows is allowed on a protected worksheet.

```javascript
getAllowDeletingRow() : boolean;
```


**Remarks**

The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

### setAllowDeletingRow(boolean) {#setAllowDeletingRow-boolean-}

Represents if the deletion of rows is allowed on a protected worksheet.

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

Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.

```javascript
getAllowFiltering() : boolean;
```


### setAllowFiltering(boolean) {#setAllowFiltering-boolean-}

Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.

```javascript
setAllowFiltering(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowFormattingCell() {#getAllowFormattingCell--}

Represents if the formatting of cells is allowed on a protected worksheet.

```javascript
getAllowFormattingCell() : boolean;
```


### setAllowFormattingCell(boolean) {#setAllowFormattingCell-boolean-}

Represents if the formatting of cells is allowed on a protected worksheet.

```javascript
setAllowFormattingCell(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowFormattingColumn() {#getAllowFormattingColumn--}

Represents if the formatting of columns is allowed on a protected worksheet

```javascript
getAllowFormattingColumn() : boolean;
```


### setAllowFormattingColumn(boolean) {#setAllowFormattingColumn-boolean-}

Represents if the formatting of columns is allowed on a protected worksheet

```javascript
setAllowFormattingColumn(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowFormattingRow() {#getAllowFormattingRow--}

Represents if the formatting of rows is allowed on a protected worksheet

```javascript
getAllowFormattingRow() : boolean;
```


### setAllowFormattingRow(boolean) {#setAllowFormattingRow-boolean-}

Represents if the formatting of rows is allowed on a protected worksheet

```javascript
setAllowFormattingRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowInsertingColumn() {#getAllowInsertingColumn--}

Represents if the insertion of columns is allowed on a protected worksheet

```javascript
getAllowInsertingColumn() : boolean;
```


### setAllowInsertingColumn(boolean) {#setAllowInsertingColumn-boolean-}

Represents if the insertion of columns is allowed on a protected worksheet

```javascript
setAllowInsertingColumn(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowInsertingHyperlink() {#getAllowInsertingHyperlink--}

Represents if the insertion of hyperlinks is allowed on a protected worksheet

```javascript
getAllowInsertingHyperlink() : boolean;
```


### setAllowInsertingHyperlink(boolean) {#setAllowInsertingHyperlink-boolean-}

Represents if the insertion of hyperlinks is allowed on a protected worksheet

```javascript
setAllowInsertingHyperlink(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowInsertingRow() {#getAllowInsertingRow--}

Represents if the insertion of rows is allowed on a protected worksheet

```javascript
getAllowInsertingRow() : boolean;
```


### setAllowInsertingRow(boolean) {#setAllowInsertingRow-boolean-}

Represents if the insertion of rows is allowed on a protected worksheet

```javascript
setAllowInsertingRow(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowSorting() {#getAllowSorting--}

Represents if the sorting option is allowed on a protected worksheet.

```javascript
getAllowSorting() : boolean;
```


### setAllowSorting(boolean) {#setAllowSorting-boolean-}

Represents if the sorting option is allowed on a protected worksheet.

```javascript
setAllowSorting(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowUsingPivotTable() {#getAllowUsingPivotTable--}

Represents if the user is allowed to manipulate pivot tables on a protected worksheet.

```javascript
getAllowUsingPivotTable() : boolean;
```


### setAllowUsingPivotTable(boolean) {#setAllowUsingPivotTable-boolean-}

Represents if the user is allowed to manipulate pivot tables on a protected worksheet.

```javascript
setAllowUsingPivotTable(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowEditingContent() {#getAllowEditingContent--}

Represents if the user is allowed to edit contents of locked cells on a protected worksheet.

```javascript
getAllowEditingContent() : boolean;
```


### setAllowEditingContent(boolean) {#setAllowEditingContent-boolean-}

Represents if the user is allowed to edit contents of locked cells on a protected worksheet.

```javascript
setAllowEditingContent(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowEditingObject() {#getAllowEditingObject--}

Represents if the user is allowed to manipulate drawing objects on a protected worksheet.

```javascript
getAllowEditingObject() : boolean;
```


### setAllowEditingObject(boolean) {#setAllowEditingObject-boolean-}

Represents if the user is allowed to manipulate drawing objects on a protected worksheet.

```javascript
setAllowEditingObject(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowEditingScenario() {#getAllowEditingScenario--}

Represents if the user is allowed to edit scenarios on a protected worksheet.

```javascript
getAllowEditingScenario() : boolean;
```


### setAllowEditingScenario(boolean) {#setAllowEditingScenario-boolean-}

Represents if the user is allowed to edit scenarios on a protected worksheet.

```javascript
setAllowEditingScenario(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getPassword() {#getPassword--}

Represents the password to protect the worksheet.

```javascript
getPassword() : string;
```


**Remarks**

If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.

### setPassword(string) {#setPassword-string-}

Represents the password to protect the worksheet.

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

Indicates whether the worksheets is protected with password.

```javascript
isProtectedWithPassword() : boolean;
```


### getAllowSelectingLockedCell() {#getAllowSelectingLockedCell--}

Represents if the user is allowed to select locked cells on a protected worksheet.

```javascript
getAllowSelectingLockedCell() : boolean;
```


### setAllowSelectingLockedCell(boolean) {#setAllowSelectingLockedCell-boolean-}

Represents if the user is allowed to select locked cells on a protected worksheet.

```javascript
setAllowSelectingLockedCell(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### getAllowSelectingUnlockedCell() {#getAllowSelectingUnlockedCell--}

Represents if the user is allowed to select unlocked cells on a protected worksheet.

```javascript
getAllowSelectingUnlockedCell() : boolean;
```


### setAllowSelectingUnlockedCell(boolean) {#setAllowSelectingUnlockedCell-boolean-}

Represents if the user is allowed to select unlocked cells on a protected worksheet.

```javascript
setAllowSelectingUnlockedCell(value: boolean) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| value | boolean | The value to set. |

### copy(Protection) {#copy-protection-}

Copy protection info.

```javascript
copy(source: Protection) : void;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| source | [Protection](/nodejs-cpp/protection/) |  |

### getPasswordHash() {#getPasswordHash--}

Gets the hash of current password.

```javascript
getPasswordHash() : number;
```


### verifyPassword(string) {#verifyPassword-string-}

Verifies password.

```javascript
verifyPassword(password: string) : boolean;
```

**Parameters:**
| Parameter | Type | Description |
| --- | --- | --- |
| password | string | The password. |


