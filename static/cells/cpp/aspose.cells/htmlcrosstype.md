##Aspose::Cells::HtmlCrossType enum
'Aspose::Cells::HtmlCrossType enum. Represents five types of html cross string in C++.'
## HtmlCrossType enum
Represents five types of html cross string.
```cpp
enum class HtmlCrossType
```
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | 0 | <br>Display like MS Excel,depends on the next cell. If the next cell is null,the string will cross,or it will be truncated. |
| MSExport | 1 | <br>Display the string like MS Excel exporting html. |
| Cross | 2 | <br>Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell. |
| CrossHideRight | 3 | <br>Display HTML cross string and hide the right string when the texts overlap. |
| FitToCell | 4 | <br>Only displaying the string within the width of cell. |
## See Also
* Namespace [Aspose::Cells](../)
* Library [Aspose.Cells for C++](../../)
