---
title: ListObject Class 
linktitle: ListObject
second_title: Aspose.Cells for Go via C++ API Reference
description: 'ListObject class. Encapsulates the object that represents listobject in Go.'
type: docs
weight: 200
url: /go-cpp/listobject/
---

## ListObject class

Represents a table in a worksheet.

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
|[GetListColumns](./getlistcolumns/) | Gets the ListColumn list of this table. | 
|[Resize](./resize/) | Resize the range of the list object. | 
|[PutCellValue_Int_Int_Object](./putcellvalue_int_int_object/) | Put the value to the cell. | 
|[PutCellValue_Int_Int_Object_Bool](./putcellvalue_int_int_object_bool/) | Put the value to the cell. | 
|[PutCellFormula_Int_Int_String](./putcellformula_int_int_string/) | Put the formula to the cell in the table. | 
|[PutCellFormula_Int_Int_String_Bool](./putcellformula_int_int_string_bool/) | Put the formula to the cell in the table. | 
|[GetShowHeaderRow](./getshowheaderrow/) | Gets and sets whether this Table shows header row. | 
|[SetShowHeaderRow](./setshowheaderrow/) | Gets and sets whether this Table shows header row. | 
|[GetShowTotals](./getshowtotals/) | Gets and sets whether this TAble shows total row. | 
|[SetShowTotals](./setshowtotals/) | Gets and sets whether this TAble shows total row. | 
|[GetDataRange](./getdatarange/) | Gets the data range of the Table. | 
|[UpdateColumnName](./updatecolumnname/) | Updates all list columns' name to cells in the table. | 
|[GetQueryTable](./getquerytable/) | Gets the linked QueryTable. | 
|[GetDataSourceType](./getdatasourcetype/) | Gets the data source type of the table. | 
|[GetHasAutoFilter](./gethasautofilter/) | Indicates whether auto filter is applied to this table. | 
|[SetHasAutoFilter](./sethasautofilter/) | Indicates whether auto filter is applied to this table. | 
|[RemoveAutoFilter](./removeautofilter/) | Removes auto filter which is applied to this table. | 
|[GetAutoFilter](./getautofilter/) | Gets auto filter of this table. | 
|[GetDisplayName](./getdisplayname/) | Gets and sets the display name of the table. | 
|[SetDisplayName](./setdisplayname/) | Gets and sets the display name of the table. | 
|[GetComment](./getcomment/) | Gets and sets the comment of the table. | 
|[SetComment](./setcomment/) | Gets and sets the comment of the table. | 
|[GetShowTableStyleFirstColumn](./getshowtablestylefirstcolumn/) | Indicates whether the first column in the table is the style applied to. | 
|[SetShowTableStyleFirstColumn](./setshowtablestylefirstcolumn/) | Indicates whether the first column in the table is the style applied to. | 
|[GetShowTableStyleLastColumn](./getshowtablestylelastcolumn/) | Indicates whether the last column in the table is the style applied to. | 
|[SetShowTableStyleLastColumn](./setshowtablestylelastcolumn/) | Indicates whether the last column in the table is the style applied to. | 
|[GetShowTableStyleRowStripes](./getshowtablestylerowstripes/) | Indicates whether row stripe formatting is applied to. | 
|[SetShowTableStyleRowStripes](./setshowtablestylerowstripes/) | Indicates whether row stripe formatting is applied to. | 
|[GetShowTableStyleColumnStripes](./getshowtablestylecolumnstripes/) | Indicates whether column stripe formatting is applied to. | 
|[SetShowTableStyleColumnStripes](./setshowtablestylecolumnstripes/) | Indicates whether column stripe formatting is applied to. | 
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
