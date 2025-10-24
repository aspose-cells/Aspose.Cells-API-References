##RenameStrategy
Strategy option for duplicate names of columns.
## RenameStrategy enumeration
Strategy option for duplicate names of columns.
### Remarks
When processing data with headers, some scenarios require the headers to be no duplication for all columns. For example, when exporting data to a datatable and the header is required to be taken as datatable's column name, duplicated values of the header are invalid. For such kind of situations, user may determine how to handle them by specifying this strategy.
### Values
| Name | Value | Description |
| --- | --- | --- |
| Exception | `0` | Throws exception. |
| Digit | `1` | Named with digit. Duplicated names will become ...1, ...2, etc. |
| Letter | `2` | Named with letter.. Duplicated names will become ...A, ...B, etc. |
