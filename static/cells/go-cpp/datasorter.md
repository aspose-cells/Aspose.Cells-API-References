##DataSorter Class
'DataSorter class. Encapsulates the object that represents datasorter in Go.'
## DataSorter class
Summary description for DataSorter.
```go
type DataSorter struct  {
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
|[GetKeys](./getkeys/) | Gets the key list of data sorter. |
|[Clear](./clear/) | Clear all settings. |
|[GetHasHeaders](./gethasheaders/) | Represents whether the range has headers. |
|[SetHasHeaders](./sethasheaders/) | Represents whether the range has headers. |
|[AddKey_Int_SortOrder](./addkey_int_sortorder/) | Adds sorted column index and sort order. |
|[AddKey_Int_SortOrder_String](./addkey_int_sortorder_string/) | Adds sorted column index and sort order with custom sort list. |
|[AddColorKey](./addcolorkey/) | Adds color sort key. |
|[AddKey_Int_SortOnType_SortOrder_Object](./addkey_int_sortontype_sortorder_object/) | Adds sorted column index and sort order with custom sort list. |
|[AddKey_Int_SortOrder_stringArray](./addkey_int_sortorder_stringarray/) | Adds sorted column index and sort order with custom sort list. |
|[GetKey1](./getkey1/) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
|[SetKey1](./setkey1/) | Represents first sorted column index(absolute position, column A is 0, B is 1, ...). |
|[GetOrder1](./getorder1/) | Represents sort order of the first key. |
|[SetOrder1](./setorder1/) | Represents sort order of the first key. |
|[GetKey2](./getkey2/) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
|[SetKey2](./setkey2/) | Represents second sorted column index(absolute position, column A is 0, B is 1, ...). |
|[GetOrder2](./getorder2/) | Represents sort order of the second key. |
|[SetOrder2](./setorder2/) | Represents sort order of the second key. |
|[GetKey3](./getkey3/) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
|[SetKey3](./setkey3/) | Represents third sorted column index(absolute position, column A is 0, B is 1, ...). |
|[GetOrder3](./getorder3/) | Represents sort order of the third key. |
|[SetOrder3](./setorder3/) | Represents sort order of the third key. |
|[GetSortLeftToRight](./getsortlefttoright/) | True means that sorting orientation is from left to right.False means that sorting orientation is from top to bottom.The default value is false. |
|[SetSortLeftToRight](./setsortlefttoright/) | True means that sorting orientation is from left to right.False means that sorting orientation is from top to bottom.The default value is false. |
|[GetCaseSensitive](./getcasesensitive/) | Gets and sets whether case sensitive when comparing string. |
|[SetCaseSensitive](./setcasesensitive/) | Gets and sets whether case sensitive when comparing string. |
|[GetSortAsNumber](./getsortasnumber/) | Indicates whether sorting anything that looks like a number. |
|[SetSortAsNumber](./setsortasnumber/) | Indicates whether sorting anything that looks like a number. |
|[Sort_Cells_Int_Int_Int_Int](./sort_cells_int_int_int_int/) | Sorts the data of the area. |
|[Sort_Cells_CellArea](./sort_cells_cellarea/) | Sort the data of the area. |
|[Sort](./sort/) | Sort the data in the range. |
