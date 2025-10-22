##Aspose::Cells::RenameStrategy enum
'Aspose::Cells::RenameStrategy enum. Strategy option for duplicate names of columns in C++.'
## RenameStrategy enum
Strategy option for duplicate names of columns.
```cpp
enum class RenameStrategy
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Exception | 0 | <br>Throws exception. |
| Digit | 1 | <br>Named with digit. Duplicated names will become ...1, ...2, etc. |
| Letter | 2 | <br>Named with letter.. Duplicated names will become ...A, ...B, etc. |
## Remarks
When processing data with headers, some scenarios require the headers to be no duplication for all columns. For example, when exporting data to a datatable and the header is required to be taken as datatable's column name, duplicated values of the header are invalid. For such kind of situations, user may determine how to handle them by specifying this strategy.
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
