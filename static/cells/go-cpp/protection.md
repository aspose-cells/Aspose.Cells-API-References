##Protection Class
'Protection class. Encapsulates the object that represents protection in Go.'
## Protection class
Represents the various types of protection options available for a worksheet.
```go
type Protection struct  {
ptr unsafe.Pointer
}
```
## Constructors
| Method | Description |
| --- | --- |
## Methods
| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. |
|[Copy](./copy/) | Copy protection info. |
|[GetAllowDeletingColumn](./getallowdeletingcolumn/) | Represents if the deletion of columns is allowed on a protected worksheet. |
|[SetAllowDeletingColumn](./setallowdeletingcolumn/) | Represents if the deletion of columns is allowed on a protected worksheet. |
|[GetAllowDeletingRow](./getallowdeletingrow/) | Represents if the deletion of rows is allowed on a protected worksheet. |
|[SetAllowDeletingRow](./setallowdeletingrow/) | Represents if the deletion of rows is allowed on a protected worksheet. |
|[GetAllowFiltering](./getallowfiltering/) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
|[SetAllowFiltering](./setallowfiltering/) | Represents if the user is allowed to make use of an AutoFilter that was created before the sheet was protected. |
|[GetAllowFormattingCell](./getallowformattingcell/) | Represents if the formatting of cells is allowed on a protected worksheet. |
|[SetAllowFormattingCell](./setallowformattingcell/) | Represents if the formatting of cells is allowed on a protected worksheet. |
|[GetAllowFormattingColumn](./getallowformattingcolumn/) | Represents if the formatting of columns is allowed on a protected worksheet |
|[SetAllowFormattingColumn](./setallowformattingcolumn/) | Represents if the formatting of columns is allowed on a protected worksheet |
|[GetAllowFormattingRow](./getallowformattingrow/) | Represents if the formatting of rows is allowed on a protected worksheet |
|[SetAllowFormattingRow](./setallowformattingrow/) | Represents if the formatting of rows is allowed on a protected worksheet |
|[GetAllowInsertingColumn](./getallowinsertingcolumn/) | Represents if the insertion of columns is allowed on a protected worksheet |
|[SetAllowInsertingColumn](./setallowinsertingcolumn/) | Represents if the insertion of columns is allowed on a protected worksheet |
|[GetAllowInsertingHyperlink](./getallowinsertinghyperlink/) | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
|[SetAllowInsertingHyperlink](./setallowinsertinghyperlink/) | Represents if the insertion of hyperlinks is allowed on a protected worksheet |
|[GetAllowInsertingRow](./getallowinsertingrow/) | Represents if the insertion of rows is allowed on a protected worksheet |
|[SetAllowInsertingRow](./setallowinsertingrow/) | Represents if the insertion of rows is allowed on a protected worksheet |
|[GetAllowSorting](./getallowsorting/) | Represents if the sorting option is allowed on a protected worksheet. |
|[SetAllowSorting](./setallowsorting/) | Represents if the sorting option is allowed on a protected worksheet. |
|[GetAllowUsingPivotTable](./getallowusingpivottable/) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
|[SetAllowUsingPivotTable](./setallowusingpivottable/) | Represents if the user is allowed to manipulate pivot tables on a protected worksheet. |
|[GetAllowEditingContent](./getalloweditingcontent/) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
|[SetAllowEditingContent](./setalloweditingcontent/) | Represents if the user is allowed to edit contents of locked cells on a protected worksheet. |
|[GetAllowEditingObject](./getalloweditingobject/) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
|[SetAllowEditingObject](./setalloweditingobject/) | Represents if the user is allowed to manipulate drawing objects on a protected worksheet. |
|[GetAllowEditingScenario](./getalloweditingscenario/) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
|[SetAllowEditingScenario](./setalloweditingscenario/) | Represents if the user is allowed to edit scenarios on a protected worksheet. |
|[GetAllowSelectingLockedCell](./getallowselectinglockedcell/) | Represents if the user is allowed to select locked cells on a protected worksheet. |
|[SetAllowSelectingLockedCell](./setallowselectinglockedcell/) | Represents if the user is allowed to select locked cells on a protected worksheet. |
|[GetAllowSelectingUnlockedCell](./getallowselectingunlockedcell/) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
|[SetAllowSelectingUnlockedCell](./setallowselectingunlockedcell/) | Represents if the user is allowed to select unlocked cells on a protected worksheet. |
|[GetPassword](./getpassword/) | Represents the password to protect the worksheet. |
|[SetPassword](./setpassword/) | Represents the password to protect the worksheet. |
|[IsProtectedWithPassword](./isprotectedwithpassword/) | Indicates whether the worksheets is protected with password. |
|[VerifyPassword](./verifypassword/) | Verifies password. |
|[GetPasswordHash](./getpasswordhash/) | Gets the hash of current password. |
