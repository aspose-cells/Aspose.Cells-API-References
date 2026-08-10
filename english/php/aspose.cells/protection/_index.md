---
title: "Protection Class"
linktitle: "Protection"
articleTitle: "Protection"
second_title: "Aspose.Cells for PHP via Java"
description: "Represents the various types of protection options available for a worksheet."
type: docs
weight: 5190
url: /php/aspose.cells/protection/
---

## Protection class

Represents the various types of protection options available for a worksheet.

## Properties

| Name | Type | Description |
| --- | --- | --- |
| [AllowDeletingColumn](#allowdeletingcolumn) | boolean | Represents if the deletion of columns is allowed on a protected worksheet. The columns containing the cells to be delete |
| [AllowDeletingRow](#allowdeletingrow) | boolean | Represents if the deletion of rows is allowed on a protected worksheet. The rows containing the cells to be deleted must |
| [AllowFiltering](#allowfiltering) | boolean | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [AllowFormattingCell](#allowformattingcell) | boolean | Represents if the formatting of cells is allowed on a protected worksheet. |
| [AllowFormattingColumn](#allowformattingcolumn) | boolean | Represents if the formatting of columns is allowed on a protected worksheet |
| [AllowFormattingRow](#allowformattingrow) | boolean | Represents if the formatting of rows is allowed on a protected worksheet |
| [AllowInsertingColumn](#allowinsertingcolumn) | boolean | Represents if the insertion of columns is allowed on a protected worksheet |
| [AllowInsertingHyperlink](#allowinsertinghyperlink) | boolean | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [AllowInsertingRow](#allowinsertingrow) | boolean | Represents if the insertion of rows is allowed on a protected worksheet |
| [AllowSorting](#allowsorting) | boolean | Represents if the sorting option is allowed on a protected worksheet. |
| [AllowUsingPivotTable](#allowusingpivottable) | boolean | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [AllowEditingContent](#alloweditingcontent) | boolean | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [AllowEditingObject](#alloweditingobject) | boolean | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [AllowEditingScenario](#alloweditingscenario) | boolean | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [AllowSelectingLockedCell](#allowselectinglockedcell) | boolean | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [AllowSelectingUnlockedCell](#allowselectingunlockedcell) | boolean | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [Password](#password) | String | Represents the password to protect the worksheet. If password is set to null or blank string, you can unprotect the work |
| [IsProtectedWithPassword](#isprotectedwithpassword) | boolean | Indicates whether the worksheets is protected with password. |

## Methods

| Name | Description |
| --- | --- |
| [copy](#copy) | Copy protection info. |
| [verifyPassword](#verifypassword) | Verifies password. |
| [getPasswordHash](#getpasswordhash) | Gets the hash of current password. |

### Protection.AllowDeletingColumn property {#allowdeletingcolumn}

Represents if the deletion of columns is allowed on a protected worksheet. The columns containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

**Type:** boolean

### Protection.AllowDeletingRow property {#allowdeletingrow}

Represents if the deletion of rows is allowed on a protected worksheet. The rows containing the cells to be deleted must be unlocked when the sheet is protected, and "Select unlocked cells" option must be enabled.

**Type:** boolean

### Protection.AllowFiltering property {#allowfiltering}

Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected.

**Type:** boolean

### Protection.AllowFormattingCell property {#allowformattingcell}

Represents if the formatting of cells is allowed on a protected worksheet.

**Type:** boolean

### Protection.AllowFormattingColumn property {#allowformattingcolumn}

Represents if the formatting of columns is allowed on a protected worksheet

**Type:** boolean

### Protection.AllowFormattingRow property {#allowformattingrow}

Represents if the formatting of rows is allowed on a protected worksheet

**Type:** boolean

### Protection.AllowInsertingColumn property {#allowinsertingcolumn}

Represents if the insertion of columns is allowed on a protected worksheet

**Type:** boolean

### Protection.AllowInsertingHyperlink property {#allowinsertinghyperlink}

Represents if the insertion of hyperlinks is allowed on a protected worksheet

**Type:** boolean

### Protection.AllowInsertingRow property {#allowinsertingrow}

Represents if the insertion of rows is allowed on a protected worksheet

**Type:** boolean

### Protection.AllowSorting property {#allowsorting}

Represents if the sorting option is allowed on a protected worksheet.

**Type:** boolean

### Protection.AllowUsingPivotTable property {#allowusingpivottable}

Represents if the user is allowed to manipulate pivot tables on a protected worksheet.

**Type:** boolean

### Protection.AllowEditingContent property {#alloweditingcontent}

Represents if the user is allowed to edit contents of locked cells on a protected worksheet.

**Type:** boolean

### Protection.AllowEditingObject property {#alloweditingobject}

Represents if the user is allowed to manipulate drawing objects on a protected worksheet.

**Type:** boolean

### Protection.AllowEditingScenario property {#alloweditingscenario}

Represents if the user is allowed to edit scenarios on a protected worksheet.

**Type:** boolean

### Protection.AllowSelectingLockedCell property {#allowselectinglockedcell}

Represents if the user is allowed to select locked cells on a protected worksheet.

**Type:** boolean

### Protection.AllowSelectingUnlockedCell property {#allowselectingunlockedcell}

Represents if the user is allowed to select unlocked cells on a protected worksheet.

**Type:** boolean

### Protection.Password property {#password}

Represents the password to protect the worksheet. If password is set to null or blank string, you can unprotect the worksheet or workbook without using a password. Otherwise, you must specify the password to unprotect the worksheet or workbook.

**Type:** String

### Protection.IsProtectedWithPassword property {#isprotectedwithpassword}

Indicates whether the worksheets is protected with password.

**Type:** boolean

### copy(source) {#copy}

Copy protection info.

| Parameter | Type | Description |
| --- | --- | --- |
| source | Protection |  |

### verifyPassword(password) {#verifypassword}

Verifies password.

| Parameter | Type | Description |
| --- | --- | --- |
| password | String | The password. |

### getPasswordHash() {#getpasswordhash}

Gets the hash of current password.
