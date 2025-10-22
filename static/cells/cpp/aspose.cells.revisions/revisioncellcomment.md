##Aspose::Cells::Revisions::RevisionCellComment class
'Aspose::Cells::Revisions::RevisionCellComment class. Represents a revision record of a cell comment change in C++.'
## RevisionCellComment class
Represents a revision record of a cell comment change.
```cpp
class RevisionCellComment : public Aspose::Cells::Revisions::Revision
```
## Methods
| Method | Description |
| --- | --- |
| [GetActionType()](./getactiontype/) | Gets the action type of the revision. |
| [GetCellName()](./getcellname/) | Gets the name of the cell. |
| [GetColumn()](./getcolumn/) | Gets the column index of the which contains a comment. |
| [GetId()](../revision/getid/) | Gets the number of this revision. |
| [GetNewLength()](./getnewlength/) | Gets Length of the comment before this revision was made. |
| [GetOldLength()](./getoldlength/) | Gets Length of the comment text added in this revision. |
| [GetRow()](./getrow/) | Gets the row index of the which contains a comment. |
| [GetType()](./gettype/) | Gets the type of revision. |
| [GetWorksheet()](../revision/getworksheet/) | Gets the worksheet. |
| [IsNull()](./isnull/) const | Checks whether the implementation object is nullptr. |
| [IsOldComment()](./isoldcomment/) | Indicates whether it's an old comment. |
| explicit [operator bool()](./operator_bool/) const | operator bool() |
| [operator=(const RevisionCellComment\& src)](./operator_asm/) | operator= |
| [operator=(const Revision\& src)](../revision/operator_asm/) | operator= |
| [Revision(Revision_Impl* impl)](../revision/revision/) | Constructs from an implementation object. |
| [Revision(const Revision\& src)](../revision/revision/) | Copy constructor. |
| [RevisionCellComment(RevisionCellComment_Impl* impl)](./revisioncellcomment/) | Constructs from an implementation object. |
| [RevisionCellComment(const RevisionCellComment\& src)](./revisioncellcomment/) | Copy constructor. |
| [RevisionCellComment(const Revision\& src)](./revisioncellcomment/) | Constructs from a parent object. |
| [SetCellName(const U16String\& value)](./setcellname/) | Gets the name of the cell. |
| [SetCellName(const char16_t* value)](./setcellname/) | Gets the name of the cell. |
| [~Revision()](../revision/~revision/) | Destructor. |
| [~RevisionCellComment()](./~revisioncellcomment/) | Destructor. |
## Fields
| Field | Description |
| --- | --- |
| [_impl](./_impl/) | The implementation object. |
## See Also
* Class [Revision](../revision/)
* Namespace [Aspose::Cells::Revisions](../)
* Library [Aspose.Cells for C++](../../)
