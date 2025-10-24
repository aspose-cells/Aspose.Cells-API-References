##ListObject Class
'ListObject class. Encapsulates the object that represents listobject in Go.'
## ListObject class
Represents a list object on a worksheet.The ListObject object is a member of the ListObjects collection.The ListObjects collection contains all the list objects on a worksheet.
```go
type ListObject struct  {
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
|[GetStartRow](./getstartrow/) | Gets the start row of the range. |
|[GetStartColumn](./getstartcolumn/) | Gets the start column of the range. |
|[GetEndRow](./getendrow/) | Gets the end  row of the range. |
|[GetEndColumn](./getendcolumn/) | Gets the end column of the range. |
|[GetListColumns](./getlistcolumns/) | Gets ListColumns of the ListObject. |
|[Resize](./resize/) | Resize the range of the list object. |
|[PutCellValue_Int_Int_Object](./putcellvalue_int_int_object/) | Put the value to the cell. |
|[PutCellValue_Int_Int_Object_Bool](./putcellvalue_int_int_object_bool/) | Put the value to the cell. |
|[PutCellFormula_Int_Int_String](./putcellformula_int_int_string/) | Put the formula to the cell in the table. |
|[PutCellFormula_Int_Int_String_Bool](./putcellformula_int_int_string_bool/) | Put the formula to the cell in the table. |
|[GetShowHeaderRow](./getshowheaderrow/) | Gets and sets whether this ListObject show header row. |
|[SetShowHeaderRow](./setshowheaderrow/) | Gets and sets whether this ListObject show header row. |
|[GetShowTotals](./getshowtotals/) | Gets and sets whether this ListObject show total row. |
|[SetShowTotals](./setshowtotals/) | Gets and sets whether this ListObject show total row. |
|[GetDataRange](./getdatarange/) | Gets the data range of the ListObject. |
|[UpdateColumnName](./updatecolumnname/) | Updates all list columns' name from the worksheet. |
|[GetQueryTable](./getquerytable/) | Gets the linked QueryTable. |
|[GetDataSourceType](./getdatasourcetype/) | Gets the data source type of the table. |
|[Filter](./filter/) | Filter the table. |
|[GetAutoFilter](./getautofilter/) | Gets auto filter. |
|[GetDisplayName](./getdisplayname/) | Gets and sets the display name. |
|[SetDisplayName](./setdisplayname/) | Gets and sets the display name. |
|[GetComment](./getcomment/) | Gets and sets the comment of the table. |
|[SetComment](./setcomment/) | Gets and sets the comment of the table. |
|[GetShowTableStyleFirstColumn](./getshowtablestylefirstcolumn/) | Indicates whether the first column in the table should have the style applied. |
|[SetShowTableStyleFirstColumn](./setshowtablestylefirstcolumn/) | Indicates whether the first column in the table should have the style applied. |
|[GetShowTableStyleLastColumn](./getshowtablestylelastcolumn/) | Indicates whether the last column in the table should have the style applied. |
|[SetShowTableStyleLastColumn](./setshowtablestylelastcolumn/) | Indicates whether the last column in the table should have the style applied. |
|[GetShowTableStyleRowStripes](./getshowtablestylerowstripes/) | Indicates whether row stripe formatting is applied. |
|[SetShowTableStyleRowStripes](./setshowtablestylerowstripes/) | Indicates whether row stripe formatting is applied. |
|[GetShowTableStyleColumnStripes](./getshowtablestylecolumnstripes/) | Indicates whether column stripe formatting is applied. |
|[SetShowTableStyleColumnStripes](./setshowtablestylecolumnstripes/) | Indicates whether column stripe formatting is applied. |
|[ApplyStyleToRange](./applystyletorange/) | Apply the table style to the range. |
|[ConvertToRange](./converttorange/) | Convert the table to range. |
|[ConvertToRange_TableToRangeOptions](./converttorange_tabletorangeoptions/) | Convert the table to range. |
|[GetTableStyleType](./gettablestyletype/) | Gets and the built-in table style. |
|[SetTableStyleType](./settablestyletype/) | Gets and the built-in table style. |
|[GetTableStyleName](./gettablestylename/) | Gets and sets the table style name. |
|[SetTableStyleName](./settablestylename/) | Gets and sets the table style name. |
|[GetXmlMap](./getxmlmap/) | Gets an XmlMap used for this list. |
|[GetAlternativeText](./getalternativetext/) | Gets and sets the alternative text. |
|[SetAlternativeText](./setalternativetext/) | Gets and sets the alternative text. |
|[GetAlternativeDescription](./getalternativedescription/) | Gets and sets the alternative description. |
|[SetAlternativeDescription](./setalternativedescription/) | Gets and sets the alternative description. |
