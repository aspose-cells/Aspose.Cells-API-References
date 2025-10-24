##RenameStrategy enumeration
## RenameStrategy enumeration
Strategy option for duplicate names of columns.
The RenameStrategy type exposes the following members:
### Fields
| Field | Description |
| :- | :- |
| EXCEPTION | Throws exception. |
| DIGIT | Named with digit. Duplicated names will become ...1, ...2, etc. |
| LETTER | Named with letter.. Duplicated names will become ...A, ...B, etc. |
### Remarks
When processing data with headers, some scenarios require the headers to be no duplication for all columns.
For example, when exporting data to a datatable and the header is required to be taken as datatable's column name,
duplicated values of the header are invalid.
For such kind of situations, user may determine how to handle them by specifying this strategy.
### See Also
* module [`aspose.cells`](..)
