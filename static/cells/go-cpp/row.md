##Row Class
'Row class. Encapsulates the object that represents row in Go.'
## Row class
Represents a single row in a worksheet.
```go
type Row struct  {
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
|[GetCellByIndex](./getcellbyindex/) | Get the cell by specific index in the cells collection of this row. |
|[IsBlank](./isblank/) | Indicates whether the row contains any data |
|[Get](./get/) | Gets the cell. |
|[GetEnumerator](./getenumerator/) | Gets the cells enumerator |
|[GetEnumerator_Bool_Bool](./getenumerator_bool_bool/) | Gets an enumerator that iterates cells through this row. |
|[GetCellOrNull](./getcellornull/) | Gets the cell or null in the specific index. |
|[IsCollapsed](./iscollapsed/) | whether the row is collapsed |
|[SetIsCollapsed](./setiscollapsed/) | whether the row is collapsed |
|[GetHeight](./getheight/) | Gets and sets the row height in unit of Points. |
|[SetHeight](./setheight/) | Gets and sets the row height in unit of Points. |
|[IsHidden](./ishidden/) | Indicates whether the row is hidden. |
|[SetIsHidden](./setishidden/) | Indicates whether the row is hidden. |
|[GetIndex](./getindex/) | Gets the index of this row. |
|[GetGroupLevel](./getgrouplevel/) | Gets the group level of the row. |
|[SetGroupLevel](./setgrouplevel/) | Gets the group level of the row. |
|[IsHeightMatched](./isheightmatched/) | Indicates whether the row height matches current default font setting of the workbook.True of this property also denotes the row height is "automatic" without custom height value set by user. |
|[SetIsHeightMatched](./setisheightmatched/) | Indicates whether the row height matches current default font setting of the workbook.True of this property also denotes the row height is "automatic" without custom height value set by user. |
|[GetStyle](./getstyle/) | Gets the style of this row. |
|[SetStyle](./setstyle/) | Sets the style of this row. |
|[GetHasCustomStyle](./gethascustomstyle/) | Indicates whether this row has custom style settings(different from the default one inherited from workbook). |
|[CopySettings](./copysettings/) | Copy settings of row, such as style, height, visibility, ...etc. |
|[GetFirstCell](./getfirstcell/) | Gets the first cell object in the row. |
|[GetFirstDataCell](./getfirstdatacell/) | Gets the first non-blank cell in the row. |
|[GetLastCell](./getlastcell/) | Gets the last cell object in the row. |
|[GetLastDataCell](./getlastdatacell/) | Gets the last non-blank cell in the row. |
|[ApplyStyle](./applystyle/) | Applies formats for a whole row. |
|[Equals_Object](./equals_object/) | Checks whether this object refers to the same row with another. |
|[Equals_Row](./equals_row/) | Checks whether this object refers to the same row with another row object. |
