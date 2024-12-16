---
title: ImportTableOptions Class 
linktitle: ImportTableOptions
second_title: Aspose.Cells for Go via C++ API Reference
description: 'ImportTableOptions class. Encapsulates the object that represents importtableoptions in Go.'
type: docs
weight: 200
url: /go-cpp/importtableoptions/
---

## ImportTableOptions class

Represents the options of importing data into cells.

```go

type ImportTableOptions struct  {
	ptr unsafe.Pointer
}

```
## Constructors

| Method | Description |
| --- | --- |
|[NewImportTableOptions](./newimporttableoptions/) | Creates the default importing options. | 

## Methods

| Method | Description |
| --- | --- |
|[IsNull](./isnull/) | Checks whether the implementation object is nullptr. | 
|[GetConvertGridStyle](./getconvertgridstyle/) | Indicates whether apply the style of the grid view to cells. | 
|[SetConvertGridStyle](./setconvertgridstyle/) | Indicates whether apply the style of the grid view to cells. | 
|[GetConvertNumericData](./getconvertnumericdata/) | Gets or sets a value that indicates whether the string value should be converted to numeric or date value. | 
|[SetConvertNumericData](./setconvertnumericdata/) | Gets or sets a value that indicates whether the string value should be converted to numeric or date value. | 
|[GetInsertRows](./getinsertrows/) | Indicates whether new rows should be added for importing data records. | 
|[SetInsertRows](./setinsertrows/) | Indicates whether new rows should be added for importing data records. | 
|[GetShiftFirstRowDown](./getshiftfirstrowdown/) | Indicates whether shifting the first row down when inserting rows. | 
|[SetShiftFirstRowDown](./setshiftfirstrowdown/) | Indicates whether shifting the first row down when inserting rows. | 
|[IsFieldNameShown](./isfieldnameshown/) | Indicates whether field name should be imported. | 
|[SetIsFieldNameShown](./setisfieldnameshown/) | Indicates whether field name should be imported. | 
|[GetExportCaptionAsFieldName](./getexportcaptionasfieldname/) | Indicates whether exporting caption as field name | 
|[SetExportCaptionAsFieldName](./setexportcaptionasfieldname/) | Indicates whether exporting caption as field name | 
|[GetDateFormat](./getdateformat/) | Gets or sets date format string for cells with imported datetime values. | 
|[SetDateFormat](./setdateformat/) | Gets or sets date format string for cells with imported datetime values. | 
|[GetTotalRows](./gettotalrows/) | Gets or sets total row count to import from data source. -1 means all rows of given data source. | 
|[SetTotalRows](./settotalrows/) | Gets or sets total row count to import from data source. -1 means all rows of given data source. | 
|[GetTotalColumns](./gettotalcolumns/) | Gets or sets total column count to import from data source. -1 means all rows of given data source. | 
|[SetTotalColumns](./settotalcolumns/) | Gets or sets total column count to import from data source. -1 means all rows of given data source. | 
|[IsHtmlString](./ishtmlstring/) | Indicates whether the value contains html tags. | 
|[SetIsHtmlString](./setishtmlstring/) | Indicates whether the value contains html tags. | 
|[GetCheckMergedCells](./getcheckmergedcells/) | Indicates whether checking merged cells. | 
|[SetCheckMergedCells](./setcheckmergedcells/) | Indicates whether checking merged cells. | 
