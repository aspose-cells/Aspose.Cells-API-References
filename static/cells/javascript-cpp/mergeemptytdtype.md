##MergeEmptyTdType
Represents the merge type for empty TD element when exporting file to html.
## MergeEmptyTdType enumeration
Represents the merge type for empty TD element when exporting file to html.
### Values
| Name | Value | Description |
| --- | --- | --- |
| Default | `0` | Display like MS Excel. |
| None | `1` | Empty TD elements will not be merged when exporting file to html. This will generate a significantly larger html file. |
| MergeForcely | `2` | Merging empty TD element forcedly when exporting file to html. The size of html file will be reduced significantly after setting value to true. If you want to import the html file to excel or export perfect grid lines when saving file to html, please keep the default value. |
