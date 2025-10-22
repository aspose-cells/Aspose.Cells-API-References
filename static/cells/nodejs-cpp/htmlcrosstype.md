##HtmlCrossType
Represents five types of html cross string.
## HtmlCrossType enumeration
Represents five types of html cross string.
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Display like MS Excel,depends on the next cell. If the next cell is null,the string will cross,or it will be truncated |
| MSExport | `1` | Display the string like MS Excel exporting html. |
| Cross | `2` | Display HTML cross string, this performance for creating large html files will be more than ten times faster than setting the value to Default or FitToCell. |
| CrossHideRight | `3` | Display HTML cross string and hide the right string when the texts overlap. |
| FitToCell | `4` | Only displaying the string within the width of cell. |
