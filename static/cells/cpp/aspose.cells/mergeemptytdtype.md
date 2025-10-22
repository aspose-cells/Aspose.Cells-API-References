##Aspose::Cells::MergeEmptyTdType enum
'Aspose::Cells::MergeEmptyTdType enum. Represents the merge type for empty TD element when exporting file to html in C++.'
## MergeEmptyTdType enum
Represents the merge type for empty TD element when exporting file to html.
```cpp
enum class MergeEmptyTdType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | 0 | <br>Display like MS Excel. |
| None | 1 | <br>Empty TD elements will not be merged when exporting file to html. This will generate a significantly larger html file. |
| MergeForcely | 2 | <br>Merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
