##Aspose::Cells::Protection class
'Aspose::Cells::Protection class. Represents the various types of protection options available for a worksheet in C++.'
## Protection class
Represents the various types of protection options available for a worksheet.
```cpp
class Protection
```
## Methods
| Method | Description |
| --- | --- |
| [Copy(const Protection\& source)](./copy/) | Copy protection info. |
| [GetAllowDeletingColumn()](./getallowdeletingcolumn/) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [GetAllowDeletingRow()](./getallowdeletingrow/) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [GetAllowEditingContent()](./getalloweditingcontent/) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [GetAllowEditingObject()](./getalloweditingobject/) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [GetAllowEditingScenario()](./getalloweditingscenario/) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [GetAllowFiltering()](./getallowfiltering/) | Represents if the user is allowed to make use of an [AutoFilter](../autofilter/) that was created before the sheet was protected. |
| [GetAllowFormattingCell()](./getallowformattingcell/) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [GetAllowFormattingColumn()](./getallowformattingcolumn/) | Represents if the formatting of columns is allowed on a protected worksheet. |
| [GetAllowFormattingRow()](./getallowformattingrow/) | Represents if the formatting of rows is allowed on a protected worksheet. |
| [GetAllowInsertingColumn()](./getallowinsertingcolumn/) | Represents if the insertion of columns is allowed on a protected worksheet. |
| [GetAllowInsertingHyperlink()](./getallowinsertinghyperlink/) | Represents if the insertion of hyperlinks is allowed on a protected worksheet. |
| [GetAllowInsertingRow()](./getallowinsertingrow/) | Represents if the insertion of rows is allowed on a protected worksheet. |
| [GetAllowSelectingLockedCell()](./getallowselectinglockedcell/) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [GetAllowSelectingUnlockedCell()](./getallowselectingunlockedcell/) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [GetAllowSorting()](./getallowsorting/) | Represents if the sorting option is allowed on a protected worksheet. |
| [GetAllowUsingPivotTable()](./getallowusingpivottable/) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [GetPassword()](./getpassword/) | Represents the password to protect the worksheet. |
| [GetPasswordHash()](./getpasswordhash/) | Gets the hash of current password. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsProtectedWithPassword()](./isprotectedwithpassword/) | Indicates whether the worksheets is protected with password. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const Protection\& src)](./operator_asm/) | operator= |
| [Protection(Protection_Impl* impl)](./protection/) | Constructs from an implementation object. |
| [Protection(const Protection\& src)](./protection/) | Copy constructor. |
| [SetAllowDeletingColumn(bool value)](./setallowdeletingcolumn/) | Represents if the deletion of columns is allowed on a protected worksheet. |
| [SetAllowDeletingRow(bool value)](./setallowdeletingrow/) | Represents if the deletion of rows is allowed on a protected worksheet. |
| [SetAllowEditingContent(bool value)](./setalloweditingcontent/) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
| [SetAllowEditingObject(bool value)](./setalloweditingobject/) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
| [SetAllowEditingScenario(bool value)](./setalloweditingscenario/) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
| [SetAllowFiltering(bool value)](./setallowfiltering/) | Represents if the user is allowed to make use of an [AutoFilter](../autofilter/) that was created before the sheet was protected. |
| [SetAllowFormattingCell(bool value)](./setallowformattingcell/) | Represents if the formatting of cells is allowed on a protected worksheet. |
| [SetAllowFormattingColumn(bool value)](./setallowformattingcolumn/) | Represents if the formatting of columns is allowed on a protected worksheet. |
| [SetAllowFormattingRow(bool value)](./setallowformattingrow/) | Represents if the formatting of rows is allowed on a protected worksheet. |
| [SetAllowInsertingColumn(bool value)](./setallowinsertingcolumn/) | Represents if the insertion of columns is allowed on a protected worksheet. |
| [SetAllowInsertingHyperlink(bool value)](./setallowinsertinghyperlink/) | Represents if the insertion of hyperlinks is allowed on a protected worksheet. |
| [SetAllowInsertingRow(bool value)](./setallowinsertingrow/) | Represents if the insertion of rows is allowed on a protected worksheet. |
| [SetAllowSelectingLockedCell(bool value)](./setallowselectinglockedcell/) | Represents if the user is allowed to select locked cells on a protected worksheet. |
| [SetAllowSelectingUnlockedCell(bool value)](./setallowselectingunlockedcell/) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
| [SetAllowSorting(bool value)](./setallowsorting/) | Represents if the sorting option is allowed on a protected worksheet. |
| [SetAllowUsingPivotTable(bool value)](./setallowusingpivottable/) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
| [SetPassword(const U16String\& value)](./setpassword/) | Represents the password to protect the worksheet. |
| [SetPassword(const char16_t* value)](./setpassword/) | Represents the password to protect the worksheet. |
| [VerifyPassword(const U16String\& password)](./verifypassword/) | Verifies password. |
| [VerifyPassword(const char16_t* password)](./verifypassword/) | Verifies password. |
| [~Protection()](./~protection/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## Examples
```cpp
Aspose::Cells::Startup();
//Instantiating a Workbook object
Workbook workbook;
Worksheet worksheet = workbook.GetWorksheets().Get(0);
//Allowing users to select locked cells of the worksheet
worksheet.GetProtection().SetAllowSelectingLockedCell(true);
//Allowing users to select unlocked cells of the worksheet
worksheet.GetProtection().SetAllowSelectingUnlockedCell(true);
Aspose::Cells::Cleanup();
```
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
