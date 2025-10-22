##Protection class
## Protection class
Represents the various types of protection options available for a worksheet.
The Protection type exposes the following members:
### Properties
| Property | Description |
| :- | :- |
| [allow_deleting_column](/cells/python-net/aspose.cells/protection/allow_deleting_column) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [allow_deleting_row](/cells/python-net/aspose.cells/protection/allow_deleting_row) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [allow_filtering](/cells/python-net/aspose.cells/protection/allow_filtering) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
| [allow_formatting_cell](/cells/python-net/aspose.cells/protection/allow_formatting_cell) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [allow_formatting_column](/cells/python-net/aspose.cells/protection/allow_formatting_column) | Represents if the formatting of columns is allowed on a protected worksheet |
| [allow_formatting_row](/cells/python-net/aspose.cells/protection/allow_formatting_row) | Represents if the formatting of rows is allowed on a protected worksheet |
| [allow_inserting_column](/cells/python-net/aspose.cells/protection/allow_inserting_column) | Represents if the insertion of columns is allowed on a protected worksheet |
| [allow_inserting_hyperlink](/cells/python-net/aspose.cells/protection/allow_inserting_hyperlink) | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
| [allow_inserting_row](/cells/python-net/aspose.cells/protection/allow_inserting_row) | Represents if the insertion of rows is allowed on a protected worksheet |
| [allow_sorting](/cells/python-net/aspose.cells/protection/allow_sorting) | Represents if the sorting option is allowed on a protected worksheet. |
| [allow_using_pivot_table](/cells/python-net/aspose.cells/protection/allow_using_pivot_table) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [allow_editing_content](/cells/python-net/aspose.cells/protection/allow_editing_content) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [allow_editing_object](/cells/python-net/aspose.cells/protection/allow_editing_object) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [allow_editing_scenario](/cells/python-net/aspose.cells/protection/allow_editing_scenario) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [allow_selecting_locked_cell](/cells/python-net/aspose.cells/protection/allow_selecting_locked_cell) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [allow_selecting_unlocked_cell](/cells/python-net/aspose.cells/protection/allow_selecting_unlocked_cell) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [password](/cells/python-net/aspose.cells/protection/password) | Represents the password to protect the worksheet. |
| [is_protected_with_password](/cells/python-net/aspose.cells/protection/is_protected_with_password) | Indicates whether the worksheets is protected with password. |
### Methods
| Method | Description |
| :- | :- |
| [`copy(self, source)`](/cells/python-net/aspose.cells/protection/copy/#aspose.cells.protection) | Copy protection info. |
| [`verify_password(self, password)`](/cells/python-net/aspose.cells/protection/verify_password/#system.string) | Verifies password. |
| [`get_password_hash(self)`](/cells/python-net/aspose.cells/protection/get_password_hash/#) | Gets the hash of current password. |
### Example
```python
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
* module [`aspose.cells`](..)
