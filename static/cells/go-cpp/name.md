##Name Class
'Name class. Encapsulates the object that represents name in Go.'
## Name class
Represents a defined name for a range of cells.
```go
type Name struct  {
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
|[GetComment](./getcomment/) | Gets and sets the comment of the name.Only applies for Excel 2007 or higher versions. |
|[SetComment](./setcomment/) | Gets and sets the comment of the name.Only applies for Excel 2007 or higher versions. |
|[GetText](./gettext/) | Gets the name text of the object. |
|[SetText](./settext/) | Gets the name text of the object. |
|[GetFullText](./getfulltext/) | Gets the name  full text of the object with the scope setting. |
|[GetRefersTo](./getrefersto/) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
|[SetRefersTo_String](./setrefersto_string/) | Returns or sets the formula that the name is defined to refer to, beginning with an equal sign. |
|[GetR1C1RefersTo](./getr1c1refersto/) | Gets or sets a R1C1 reference of the Name. |
|[SetR1C1RefersTo](./setr1c1refersto/) | Gets or sets a R1C1 reference of the Name. |
|[GetRefersTo_Bool_Bool](./getrefersto_bool_bool/) | Get the reference of this Name. |
|[GetRefersTo_Bool_Bool_Int_Int](./getrefersto_bool_bool_int_int/) | Get the reference of this Name based on specified cell. |
|[SetRefersTo_String_Bool_Bool](./setrefersto_string_bool_bool/) | Set the reference of this Name. |
|[IsReferred](./isreferred/) | Indicates whether this name is referred by other formulas. |
|[IsVisible](./isvisible/) | Indicates whether the name is visible. |
|[SetIsVisible](./setisvisible/) | Indicates whether the name is visible. |
|[GetSheetIndex](./getsheetindex/) | Indicates this name belongs to Workbook or Worksheet.0 = Global name, otherwise index to sheet (one-based) |
|[SetSheetIndex](./setsheetindex/) | Indicates this name belongs to Workbook or Worksheet.0 = Global name, otherwise index to sheet (one-based) |
|[ToString](./tostring/) | Returns a string represents the current Range object. |
|[GetRanges](./getranges/) | Gets all ranges referred by this name. |
|[GetRanges_Bool](./getranges_bool/) | Gets all ranges referred by this name. |
|[GetReferredAreas](./getreferredareas/) | Gets all references referred by this name. |
|[GetRange](./getrange/) | Gets the range if this name refers to a range. |
|[GetRange_Bool](./getrange_bool/) | Gets the range if this name refers to a range |
|[GetRange_Int_Int_Int](./getrange_int_int_int/) | Gets the range if this name refers to a range.If the reference of this name is not absolute, the range may be different for different cell. |
