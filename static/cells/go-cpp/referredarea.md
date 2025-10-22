##ReferredArea Class
'ReferredArea class. Encapsulates the object that represents referredarea in Go.'
## ReferredArea class
Represents a referred area by the formula.
```go
type ReferredArea struct  {
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
|[IsExternalLink](./isexternallink/) | Indicates whether this is an external link. |
|[GetExternalFileName](./getexternalfilename/) | Get the external file name if this is an external reference. |
|[GetSheetName](./getsheetname/) | Indicates which sheet this reference is in. |
|[GetSheetNames](./getsheetnames/) | Names of all the worksheets this instance references to. |
|[IsEntireRow](./isentirerow/) | Indicates whether this area contains all columns(entire row). |
|[IsEntireColumn](./isentirecolumn/) | Indicates whether this area contains all rows(entire column). |
|[IsArea](./isarea/) | Indicates whether this is an area. |
|[GetEndColumn](./getendcolumn/) | The end column of the area. |
|[GetStartColumn](./getstartcolumn/) | The start column of the area. |
|[GetEndRow](./getendrow/) | The end row of the area. |
|[GetStartRow](./getstartrow/) | The start row of the area. |
|[GetValues](./getvalues/) | Gets cell values in this area. |
|[GetValues_Bool](./getvalues_bool/) | Gets cell values in this area. |
|[GetValue_Int_Int](./getvalue_int_int/) | Gets cell value with given offset from the top-left of this area. |
|[GetValue_Int_Int_Bool](./getvalue_int_int_bool/) | Gets cell value with given offset from the top-left of this area. |
|[ToString](./tostring/) | Returns the reference address of this area.Generally it is the address of the reference which may be used in formula, such as "Sheet1!A1:C3". |
