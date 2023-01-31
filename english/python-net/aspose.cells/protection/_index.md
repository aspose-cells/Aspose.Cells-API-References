---
title: Protection class
second_title: Aspose.Cells for Python via .NET API References
description: 
type: docs
weight: 1220
url: /python-net/aspose.cells/protection/
is_root: false
---

## Protection class

Represents the various types of protection options available for a worksheet.



The Protection type exposes the following members:

### Properties
| Property | Description |
| :- | :- |
| [allow_deleting_column](/cells/python-net/aspose.cells/protection/allow_deleting_column) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [is_deleting_columns_allowed](/cells/python-net/aspose.cells/protection/is_deleting_columns_allowed) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [allow_deleting_row](/cells/python-net/aspose.cells/protection/allow_deleting_row) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [is_deleting_rows_allowed](/cells/python-net/aspose.cells/protection/is_deleting_rows_allowed) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [allow_filtering](/cells/python-net/aspose.cells/protection/allow_filtering) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [is_filtering_allowed](/cells/python-net/aspose.cells/protection/is_filtering_allowed) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [allow_formatting_cell](/cells/python-net/aspose.cells/protection/allow_formatting_cell) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [is_formatting_cells_allowed](/cells/python-net/aspose.cells/protection/is_formatting_cells_allowed) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [allow_formatting_column](/cells/python-net/aspose.cells/protection/allow_formatting_column) | Represents if the formatting of columns is allowed on a protected worksheet |
| [is_formatting_columns_allowed](/cells/python-net/aspose.cells/protection/is_formatting_columns_allowed) | Represents if the formatting of columns is allowed on a protected worksheet |
| [allow_formatting_row](/cells/python-net/aspose.cells/protection/allow_formatting_row) | Represents if the formatting of rows is allowed on a protected worksheet |
| [is_formatting_rows_allowed](/cells/python-net/aspose.cells/protection/is_formatting_rows_allowed) | Represents if the formatting of rows is allowed on a protected worksheet |
| [allow_inserting_column](/cells/python-net/aspose.cells/protection/allow_inserting_column) | Represents if the insertion of columns is allowed on a protected worksheet |
| [is_inserting_columns_allowed](/cells/python-net/aspose.cells/protection/is_inserting_columns_allowed) | Represents if the insertion of columns is allowed on a protected worksheet |
| [allow_inserting_hyperlink](/cells/python-net/aspose.cells/protection/allow_inserting_hyperlink) | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [is_inserting_hyperlinks_allowed](/cells/python-net/aspose.cells/protection/is_inserting_hyperlinks_allowed) | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [allow_inserting_row](/cells/python-net/aspose.cells/protection/allow_inserting_row) | Represents if the insertion of rows is allowed on a protected worksheet |
| [is_inserting_rows_allowed](/cells/python-net/aspose.cells/protection/is_inserting_rows_allowed) | Represents if the insertion of rows is allowed on a protected worksheet |
| [allow_sorting](/cells/python-net/aspose.cells/protection/allow_sorting) | Represents if the sorting option is allowed on a protected worksheet. |
| [is_sorting_allowed](/cells/python-net/aspose.cells/protection/is_sorting_allowed) | Represents if the sorting option is allowed on a protected worksheet. |
| [allow_using_pivot_table](/cells/python-net/aspose.cells/protection/allow_using_pivot_table) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [is_using_pivot_tables_allowed](/cells/python-net/aspose.cells/protection/is_using_pivot_tables_allowed) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [allow_editing_content](/cells/python-net/aspose.cells/protection/allow_editing_content) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [is_editing_contents_allowed](/cells/python-net/aspose.cells/protection/is_editing_contents_allowed) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [allow_editing_object](/cells/python-net/aspose.cells/protection/allow_editing_object) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [is_editing_objects_allowed](/cells/python-net/aspose.cells/protection/is_editing_objects_allowed) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [allow_editing_scenario](/cells/python-net/aspose.cells/protection/allow_editing_scenario) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [is_editing_scenarios_allowed](/cells/python-net/aspose.cells/protection/is_editing_scenarios_allowed) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [password](/cells/python-net/aspose.cells/protection/password) | Represents the password to protect the worksheet. |
| [is_protected_with_password](/cells/python-net/aspose.cells/protection/is_protected_with_password) | Indicates whether the worksheets is protected with password. |
| [allow_selecting_locked_cell](/cells/python-net/aspose.cells/protection/allow_selecting_locked_cell) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [is_selecting_locked_cells_allowed](/cells/python-net/aspose.cells/protection/is_selecting_locked_cells_allowed) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [allow_selecting_unlocked_cell](/cells/python-net/aspose.cells/protection/allow_selecting_unlocked_cell) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [is_selecting_unlocked_cells_allowed](/cells/python-net/aspose.cells/protection/is_selecting_unlocked_cells_allowed) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |


### Methods
| Method | Description |
| :- | :- |
| [copy(source)](/cells/python-net/aspose.cells/protection/copy/#Protection) | Copy protection info. |
| [get_password_hash()](/cells/python-net/aspose.cells/protection/get_password_hash/#) | Gets the hash of current password. |
| [verify_password(password)](/cells/python-net/aspose.cells/protection/verify_password/#str) | Verifies password. |


### Example 


```
from aspose.cells import Workbook

# Instantiating a Workbook object
workbook = Workbook()
worksheet = workbook.worksheets[0]

# Allowing users to select locked cells of the worksheet
worksheet.protection.allow_selecting_locked_cell = True

# Allowing users to select unlocked cells of the worksheet
worksheet.protection.allow_selecting_unlocked_cell = True

```
### See Also

* module [aspose.cells](../)
