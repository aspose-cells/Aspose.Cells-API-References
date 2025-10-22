##AutoFilter Class
'AutoFilter class. Encapsulates the object that represents autofilter in Go.'
## AutoFilter class
Represents autofiltering for the specified worksheet.
```go
type AutoFilter struct  {
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
|[GetSorter](./getsorter/) | Gets the data sorter. |
|[SetRange_Int_Int_Int](./setrange_int_int_int/) | Sets the range to which the specified AutoFilter applies. |
|[GetCellArea](./getcellarea/) | Gets the CellArea where the this AutoFilter applies to. |
|[GetCellArea_Bool](./getcellarea_bool/) | Gets the CellArea where the specified AutoFilter applies to. |
|[GetRange](./getrange/) | Represents the range to which the specified AutoFilter applies. |
|[SetRange_String](./setrange_string/) | Represents the range to which the specified AutoFilter applies. |
|[AddFilter](./addfilter/) | Adds a filter for a filter column. |
|[AddDateFilter](./adddatefilter/) | Adds a date filter. |
|[RemoveDateFilter](./removedatefilter/) | Removes a date filter. |
|[RemoveFilter_Int_String](./removefilter_int_string/) | Removes a filter for a filter column. |
|[Filter](./filter/) | Filters a list with specified criteria. |
|[FilterTop10](./filtertop10/) | Filter the top 10 item in the list |
|[Dynamic_Filter](./dynamic_filter/) | Adds a dynamic filter. |
|[AddFontColorFilter](./addfontcolorfilter/) | Adds a font color filter. |
|[AddFillColorFilter](./addfillcolorfilter/) | Adds a fill color filter. |
|[AddIconFilter](./addiconfilter/) | Adds an icon filter. |
|[MatchBlanks](./matchblanks/) | Match all blank cell in the list. |
|[MatchNonBlanks](./matchnonblanks/) | Match all not blank cell in the list. |
|[Custom_Int_FilterOperatorType_Object](./custom_int_filteroperatortype_object/) | Filters a list with a custom criteria. |
|[Custom_Int_FilterOperatorType_Object_Bool_FilterOperatorType_Object](./custom_int_filteroperatortype_object_bool_filteroperatortype_object/) | Filters a list with custom criteria. |
|[ShowAll](./showall/) | Unhide all rows. |
|[RemoveFilter_Int](./removefilter_int/) | Remove the specific filter. |
|[Refresh](./refresh/) | Refresh auto filters to hide or unhide the rows. |
|[Refresh_Bool](./refresh_bool/) | Gets all hidden rows' indexes. |
|[GetShowFilterButton](./getshowfilterbutton/) | Indicates whether the AutoFilter button for this column is visible. |
|[SetShowFilterButton](./setshowfilterbutton/) | Indicates whether the AutoFilter button for this column is visible. |
|[GetFilterColumns](./getfiltercolumns/) | Gets the collection of the filter columns. |
